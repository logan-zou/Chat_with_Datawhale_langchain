# hands-dirty-nlp
- 课程前置要求：默认已完成<必修课程>
- 定位及目的：本课程面对具有一定机器学习基础，但尚未入门的NLPer或经验尚浅的NLPer，尽力避免陷入繁琐枯燥的公式讲解中，力求用代码展示每个模型背后的设计思想，同时也会带大家梳理每个模块下的技术演变，做到既知树木也知森林。

## 课程目录
### 文本表示
- 任务定义：文本表示是把现实中的文本数据转化为计算机能够运算的数值向量，这样就可以针对文本信息进行计算，进而来完成各种NLP任务。本章将介绍文本表示的演进过程，基于此大家也可对NLP的发展历程有一个基本了解。
- 离散表示：one-hot、bag-of-word、tf-idf
- 稠密表示-词向量：word2vec、glove
- 预训练系列：
- 初识预训练模型：elmo
  - 自编码：bert、ernie等
  - 自回归：gpt等
  - Prompt
- 发展脉络

### 序列标注
- 任务定义：序列标注的涵盖范围很广泛，可用于解决一系列对token进行分类的问题，如分词、命名实体识别、词性标注等。本章以命名实体识别为切入点，介绍序列标注任务的前世今生。
- NER
  - 任务简介：标注方式、评价指标
  - 传统方法：词典匹配、CRF、HMM
  - 深度学习方法：LSTM + CRF、BERT+CRF
  - 融入词汇的方法：lattice、FLAT、LEBERT（位置编码在NER的重要性）
  - 解码方式：softmax、CRF、span-pointer、片段排列
- flat-NER
- nested-NER
- 发展脉络

### 分类任务
- 任务定义：分类任务是NLP中应用最多的任务，在工业界很多实际业务问题都可以抽象成分类任务。本章以意图识别为切入点，介绍分类任务的经典方法。
- 意图识别：
  - 任务简介：评价指标
  - 经典深度学习方法：fasttext、text-cnn、lstm
  - 基于预训练模型的方法：bert
- 解码:
  - 单标签
  - 多标签
- 发展脉络

### 文本匹配
- 任务定义：文本匹配是为了判断两个文本之间的相关关系，不同的场景下对”相关的“的定义是不同的，例如：qq匹配（query-query）：对话任务中，判断两个问句是否相似；qa匹配（query-answer）：对话任务中，判断用户问句与回复是否对应；qt匹配（query-title）：搜索任务中，判断用户的输入和文章标题是否相关。本小节以qq切入点，介绍匹配任务方法的演进。
- qq匹配
  - 任务简介
  - 双塔：优缺点
    - dssm
    - bert双塔
  - 交互：优缺点
    - ESIM
    - simbert
- 发展脉络

### 生成任务
- 任务定义： 文本生成是NLP中较为复杂的任务，本章只聚焦于文本到文本的生成，例如生成式摘要、机器翻译、对话生成等等。本文以其中的对话生成和机器翻译为切入点，介绍其中的经典方法。
- 对话生成
  - 任务简介
  - 方法：bert-base-s2s、gpt
- 机器翻译
  - 任务简介
  - 方法：rnn-base-s2s、bert-base-s2s
- 发展脉络

### 阅读理解
- 任务定义：相对于其他NLP任务，阅读理解侧重于深入理解文档中的语义信息，一般来说包含完型填空、多项选择、答案抽取、自由问答这4个任务。本章以其中的多项选择与答案抽取作为切入点，介绍其中的经典方法。
- 多项选择
  - 任务简介
  - 方法
- 答案抽取
  - 任务简介
- 方法
- 发展脉络

## 贡献者名单
| 姓名 | 个人简介 | 个人主页 |
| :----| :---- | :---- |
| 慎独 | NLP算法工程师，项目负责人 | - |
| 西瓜骑士 | NLP算法工程师，项目负责人 | - |
| 芙蕖 | NLP算法工程师 | - |


## 关注我们
<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "180" height = "180">
</div>

## LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。
