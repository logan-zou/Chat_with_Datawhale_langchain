# Sweettalk-Django4.2

## 项目介绍

Django 是一个使用 Python 编写的开源 Web 应用程序框架，它提供了一套用于快速开发安全、
可扩展和高效的 Web 应用程序的工具和功能。Django 基于 MVC（Model-View-Controller）架构模式，采用了最佳实践，强调代码的可重用性和可维护性。它的设计理念是 DRY（Don't Repeat Yourself），
通过提供许多内置功能和现成的解决方案，使开发人员能够专注于业务逻辑而不必从头开始构建所有组件。此次开源项目旨在为大家讲解基础的 Django 项目创建，
以及简单程序的编写。  

该项目示例是一个商品入库和查询系统，通过我们构建的数据表，将商品的详细信息入库存储，并且可以按条件过滤查询数据，获取详细商品或者商品品类的信息。

**[学习地址](https://joe-2002.github.io/sweettalk-django4.2/)**

## 项目受众

1. 开发人员和程序员：Django 是一个流行的 Web 框架，许多开发人员和程序员选择使用它来快速构建可扩展的 Web 应用程序。无论是有经验的开发人员还是初学者，Django 都提供了一个强大且易于使用的平台来创建功能丰富的网站和应用。

2. 学生和教育机构：许多大学、学院和教育机构将 Django 作为教学的一部分，因为它简单易懂，同时又涵盖了 Web 开发的各个方面。学生可以通过学习 Django 来获得实际的编程经验，并将其应用到项目中。

3. 创业者和企业家：对于有创业想法或开设在线业务的人来说，Django 是一个理想的选择。它提供了一个稳定、可靠且高效的开发平台，可以帮助他们快速构建起自己的网站或应用程序，并提供必要的功能和工具来支持业务的发展。

4. Web 设计师和 UI/UX 设计师：尽管 Django 是一个后端框架，但在开发过程中，与前端设计师和 UI/UX 设计师密切合作是非常重要的。Django 提供了与前端技术（如 HTML、CSS 和 JavaScript）的无缝集成，并允许设计师将设计和用户体验融入到 Web 应用中。

## 基本信息

学习周期：8 天，每天平均花费时间 1 小时-2 小时不等，根据个人学习接受能力强弱有所浮动。

学习形式：理论学习 + 练习

人群定位：可以零基础入门。

难度系数：容易

备注：需要 Python 基础

如果觉得本项目中有错误，可以[点击这里](https://github.com/Joe-2002/sweettalk_django4.2/issues)提交你希望补充的内容，我们看到后会尽快进行补充。

## 项目亮点

1.本项目拥有清晰简洁的教学文档和匹配的课后习题。

2.项目开发过程中会涉及到设计、开发、调试、部署等多个环节，这将使你熟悉整个 Web 应用的生命周期。

## DataWhale开源学习记录     
| 时间      | 人数 |
| ----------- | ------ |
| 2023年8月 | 55人 |
| 待定      |      |     

**共计55人**

## 项目规划

### Day1

#### 虚拟环境

1. 在虚拟环境中，安装 debug_toolbar 库
2. 在虚拟环境中，安装 django_extensions 库

#### 搭建项目

1. 新建一个名为 erp 的项目
2. 在 apps 中，新建名为 data 的 app
3. 在 apps 中，新建名为 purchase 的 app

#### 运行项目

1. 配置 settings.py 文件
2. 运行项目

### Day2

#### 构建数据表并合并

1. 创建产品分类和产品两个数据表
2. 执行生成迁移脚本命令（python manage.py makemigrations）和迁移命令（python manage.py migrate）

#### 据表的常用字段和常用配置

1. 熟悉数据表的常用字段和常用配置
2. 尝试使用数据表的字段和配置

### Day3

#### 引入 admin 后台和管理员

1. 创建 admin 的超级管理员
2. 在 admin 文件中引入数据表
3. 注册数据表到 admin

#### 外键的使用

1. 给产品表创建一个外键
2. 撰写根据产品分类筛选产品的 api
3. 使用 postman 调用 api

### Day4

#### QuerySet 和 Instance

1. 输出相关数据的数据类型，找出 QuerySet 和 Instance
2. 尝试对数据进行增删查改等操作

### Day5

#### APIView

1. 使用 APIView，试比较 APIView 和 as_view 的区别
2. 使用 APIView 的 as_view 方法

### Day6

#### 构建序列化

1. 构建序列化
2. 序列化单个字段
3. 序列化多个字段
4. 序列化所有字段

#### 序列化的高级使用

1. 序列化单个对象
2. 序列化多个对象
3. 序列关联对象（有外键）

### Day7

#### Django-DRF(ModelViewSet)的使用

1. Django-DRF（ModelViewSet）简介
2. 使用 DRF（ModelViewSet）方法

### Day8

#### DefaultRouter 的使用

1. 导入 DefaultRouter
2. 使用 DefaultRouter 注册 API
3. 将 API 导入项目路由配置中

#### 自定义函数的使用

1. 引入自定义函数的装饰器
2. 编写自定义函数
3. 测试自定义函数

## 贡献者

项目负责人：[李柯辰](https://github.com/Joe-2002)

邮箱：likechen@linchance.com

<div>
<table border="0">
  <tbody>
    <tr align="center" >
      <td>
         <a href="https://github.com/Joe-2002"><img width="70" height="70" src="https://github.com/Joe-2002.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/Joe-2002">李柯辰</a> 
        <p> 南京航空航天大学<br>江苏霖承科技有限公司</p>
      </td>
      <td>
         <a href="https://github.com/zhumengyu"><img width="70" height="70" src="https://github.com/zhumengyu.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/zhumengyu">朱梦雨</a> 
        <p>南通理工学院<br>江苏霖承科技有限公司</p>
      </td>
      <td>
         <a href="https://github.com/Ethan-2004"><img width="70" height="70" src="https://github.com/Ethan-2004.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/Ethan-2004">张海生</a>
         <p>南通师范高等专科学校<br>江苏霖承科技有限公司</p>
      </td>
    </tr>
  </tbody>
</table>
</div>

## 致谢

特别感谢 [@Sm1les](https://github.com/Sm1les)、[胡锐锋](https://github.com/Relph1119)对本项目的帮助与支持。

特别感谢以下为教程做出贡献的同学！

<a href="https://github.com/Joe-2002/sweettalk-django4.2/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Joe-2002/sweettalk-django4.2" />
</a>



## 项目地址

[点击这里](https://github.com/Joe-2002/sweettalk_django4.2)

## License
LinChance © 2023, sweettalk-django4.2 - Released under the GNU General Public License v3.0





