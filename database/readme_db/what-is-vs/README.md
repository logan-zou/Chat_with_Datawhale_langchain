# What is Vector Search

![DALL-E](./images/DALL-E.png)
<div align=center>
<p>Made by DALL·E</p>
</div>

本项目旨在创建一个全面、易于理解的向量检索教程，它将覆盖从基础理论到核心技术的各个方面。教程将通过详细的解释、实例和实践案例，帮助初学者、研究人员以及应用人员深入理解并有效地使用向量检索技术。

## 项目受众

- 初学者，希望从基础了解向量检索。
- 相关领域的研究人员，需要了解最新技术和应用。
- 应用人员，需要实际开发应用向量检索技术。

## Roadmap

- 第一部分：引言和基础知识
  - [引言](./docs/chapter1/introduction.md)
    - 什么是向量检索
    - 为什么向量检索重要
    - 教程目标和读者指南
  - [向量检索的历史和发展](./docs/chapter1/history.md)
    - 早期的信息检索方法
    - 从传统检索到向量检索的演进
  - [基本概念](./docs/chapter1/basic.md)
    - 向量空间和维度
    - 向量化的数据表示
    - 相似性度量基础

- 第二部分：核心技术
  - [向量化技术](./docs/chapter2/embedding.md)
    - 非结构化数据
    - 非结构化数据向量化
  - 向量索引
    - [向量索引概述](./docs/chapter2/index.md)
      - 概述
      - 评估技术
    - [基于量化的向量索引方法](./docs/chapter2/pq-based-index.md)
    - [基于哈希的向量索引方法](./docs/chapter2/hash-based-index.md)
    - [基于树的向量索引方法](./docs/chapter2/tree-based-index.md)
    - [基于图的向量索引方法](./docs/chapter2/graph-based-index.md)
    - [基于混合的向量索引方法](./docs/chapter2/hybrid-index.md)
  - [混合查询](./docs/chapter2/hybrid-search.md)
  - [向量索引优化策略](./docs/chapter2/index-tuning.md)
    - 查询负载驱动的参数优化策略
    - 数据驱动的空间划分策略
    - 基于硬件加速的向量索引方法

- 第三部分：系统实现与应用
  - [向量数据库系统概述](./docs/chapter3/system.md)
    - 向量数据库的基本构成与工作原理
    - 市面主流向量数据库系统比较
  - [案例研究](./docs/chapter3/case.md)
    - [专有型向量数据库实践](./docs/chapter3/system-case-special.md)
    - [拓展型向量数据库实践](./docs/chapter3/system-case-expand.md)

- 第四部分：未来展望和挑战
  - [新兴技术趋势](./docs/chapter4/ternd.md)
    - [神经网络与向量检索的结合](./docs/chapter4/NN-index.md)
    - [Learned Index](./docs/chapter4/learned-index.md)
    - [DB4LLM](./docs/chapter4/DB4LLM.md)
    - [RAG 架构初探](./docs/chapter4/RAG.md)
  - [面临的挑战](./docs/chapter4/challenge.md)
    - 数据隐私和安全问题
    - 行业发展趋势和未来应用场景

- [结语](./docs/summary.md)
  - 总结
  - 附录：进一步阅读资源和工具列表

## 参与贡献

- 如果你想参与到项目中来欢迎查看项目的 [Issue](https://github.com/datawhalechina/what-is-vs/issues) 查看没有被分配的任务。
- 如果你发现了一些问题，欢迎在 [Issue](https://github.com/datawhalechina/what-is-vs/issues) 中进行反馈🐛。

如果你对 Datawhale 很感兴趣并想要发起一个新的项目，欢迎查看 [Datawhale 贡献指南](https://github.com/datawhalechina/DOPMC#%E4%B8%BA-datawhale-%E5%81%9A%E5%87%BA%E8%B4%A1%E7%8C%AE)。

## 贡献者名单

| 姓名 | 职责 | 简介 |
| :----| :---- | :---- |
| [苏鹏](https://github.com/SuperSupeng) | 项目负责人 | Datawhale成员 |
| [李剑楠]((https://github.com/)ljn-aaa) | 项目主要贡献者 | 华东师范大学硕士 |
| [向隆](https://github.com/BenjaminXiang) | 项目主要贡献者 | 南方科技大学博士 |
| 王泽宇 | 项目主要贡献者 | 复旦大学博士 |
| [王梦召](https://github.com/whenever5225) | 项目主要贡献者 | 浙江大学博士 |
| [田冰](https://github.com/tianbing111) | 项目主要贡献者 | 华中科技大学博士 |
| [韩颐堃](https://github.com/YikunHan42) | 项目主要贡献者 |  |

分工请见：[立项申请（what-is-vs #184）](https://github.com/datawhalechina/DOPMC/issues/184)

## 关注我们

<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "180" height = "180">
</div>

## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。