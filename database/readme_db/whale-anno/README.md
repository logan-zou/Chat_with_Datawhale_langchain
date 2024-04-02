# whaleAnno

Datawhale自研数据标注工具

## 功能开发进度

- NLP：
  - [X] 命名实体识别
  - [X] 文本分类
  - [X] 人类反馈强化学习
  - [X] 关系标注
- CV：
  - [X] 关键点
  - [X] 图像分类
  - [ ] 目标检测
  - [ ] 图像分割

## 快速开始

### 环境配置

#### Python 3

经测试whaleAnno后端代码可在Python 3.7.9上运行，您也可以测试其他版本，一般建议安装最新版

### 克隆项目

```shell
git clone https://github.com/datawhalechina/whale-anno.git
```

### 安装依赖

```shell
# 下载后端依赖
python3 -m pip install flask==2.0.0
```

后端只依赖了flask这个第三方库

### 启动项目

打开终端

```shell
# 进入后端目录
cd ./be
# 启动后端脚本
python3 ./run.py
```

此时项目会被启动在http://localhost:9060/index.html

### 开始使用

打开上述地址，然后点击[这里](https://www.bilibili.com/video/BV1v64y197iA?p=2)查看使用教程。此外，我们还提供了一个用于临时标注少量数据的单机版本（目前仅支持Windows），点击[这里](https://github.com/datawhalechina/whale-anno/releases)去下载，点击[这里](https://www.bilibili.com/video/BV1v64y197iA?p=1)查看单机版使用教程

## 开发团队

|      职责      |                  名单                  |
| :------------: | :-------------------------------------: |
|  **PM**  |    [谢文睿](https://github.com/Sm1les)    |
| **前端** |  [马琦钧](https://github.com/Skypow2012)  |
| **后端** | [张翔宇](https://github.com/xgdyp)、付文豪 |

## 关注我们

<div align=center>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "250" height = "270" alt="Datawhale是一个专注AI领域的开源组织，以“for the learner，和学习者一起成长”为愿景，构建对学习者最有价值的开源学习社区。关注我们，一起学习成长。">
</div>

## LICENSE

`<img style="border-width:0" src="https://img.shields.io/badge/license-GPL--3.0-lightgrey" /><br />`本作品采用GNU General Public License v3.0进行许可。
