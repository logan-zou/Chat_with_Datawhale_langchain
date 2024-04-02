# 基于Arrow的轻量内存池

这个项目的内存池是基于[Apache Arrow项目](https://github.com/apache/arrow)的衍生版本。我们将Arrow项目中复杂的核心结构——内存池——完全剥离出来，形成了这个独立的项目。由于原始的内存池与Arrow项目本身的工具有深度依赖关系，因此我们在这个项目中对内存池进行了一些深度移除和改造，以保持与原始Arrow内存池的基础功能一致。一些改动包括：

- 分离allocator与memory_pool
- 移除不需要的LoggingMemoryPool、ProxyMemoryPool
- 移除jemalloc等第三方malloc库，未来可以支持

通过这些改动，我们的目标是：

- 使代码更加精简
- 使内存池更方便地作为其他项目的依赖库使用
- 提供简单的方式来引入本项目的so库和头文件，以使用内存池功能

此外，这个项目还可以作为深入学习内存池设计与实现的资源。我们欢迎您探索并使用这个经过精心改进的内存池。

## 1.如何编译

```
➜  bazel build //src:memory_pool 
WARNING: Ignoring JAVA_HOME, because it must point to a JDK, not a JRE.
WARNING: Ignoring JAVA_HOME, because it must point to a JDK, not a JRE.
INFO: Analyzed target //src:memory_pool (36 packages loaded, 169 targets configured).
INFO: Found 1 target...
Target //src:memory_pool up-to-date:
  bazel-bin/src/libmemory_pool.a
  bazel-bin/src/libmemory_pool.dylib
INFO: Elapsed time: 1.568s, Critical Path: 1.05s
INFO: 10 processes: 4 internal, 6 darwin-sandbox.
INFO: Build completed successfully, 10 total actions
```

## 2.如何使用

所有的用例放在[examples目录](./examples/)

### 2.1 编写一个简单的case

参见：[helloworld](./examples/hello_world.cc)

```cpp
arrow::MemoryPool* pool = arrow::default_memory_pool();

char* val;
arrow::Status status = pool->Allocate(14, reinterpret_cast<uint8_t**>(&val));

if (status.ok()) {
    std::cout << "Memory allocation successful." << std::endl;
    std::strcpy(val, "Hello, World!");
    std::cout << "Filled content: " << val << std::endl;
    pool->Free(reinterpret_cast<uint8_t*>(val), 4);
} else {
    std::cout << "Memory allocation failed." << std::endl;
}
```

编译：
```cpp
➜  bazel build //examples:hello_world 
WARNING: Ignoring JAVA_HOME, because it must point to a JDK, not a JRE.
WARNING: Ignoring JAVA_HOME, because it must point to a JDK, not a JRE.
INFO: Analyzed target //examples:hello_world (0 packages loaded, 2 targets configured).
INFO: Found 1 target...
Target //examples:hello_world up-to-date:
  bazel-bin/examples/hello_world
INFO: Elapsed time: 0.881s, Critical Path: 0.73s
INFO: 7 processes: 5 internal, 2 darwin-sandbox.
INFO: Build completed successfully, 7 total actions
```

运行：
```cpp
➜  bazel-bin/examples/hello_world
Memory allocation successful.
Filled content: Hello, World!
```

## 3.如何测试

测试基于catch2编写，所有测试位于[tests目录](./tests/)

可以测试tests目录下面的其他测试，只需要替换submit_test为对应的test即可。

```cpp
bazel test //tests:memory_pool_test
```
