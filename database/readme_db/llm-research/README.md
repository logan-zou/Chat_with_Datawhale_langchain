# LLM Research
<img src="./images/readme1.png" alt="image-20231130085512212" width="1000" />

> Enjoy LLM.

## 项目简介

我们致力于建立一个LLM论文解读笔记仓库，我们将集结LLM领域的经典论文，然后为这些论文提供解读笔记。

通过LLM Research，研究人员可以迅速查阅到LLM领域的重要论文，无需费时费力地查找和筛选。此外，针对(只想粗略浏览LLM领域学术前沿的核心思想的)其他方向的研究人员，本仓库也提供了这些重点论文的相应解读笔记(每篇笔记分为TLDR简版和精读版)，让这部分研究人员必须不花时间去细读每篇原文。

我们已经初步组建好写作小组，并计划于近期三四个月撰写好相应文章的精读笔记。

## 项目受众
- 想细致学习LLM学习前沿的同学们。
- 对大模型科研感兴趣的研究人员。
- 仅需要对深度学习和NLP有基本了解。

## 项目亮点
大型语言模型在当今技术领域占据重要地位，其在自然语言处理、文本生成、信息检索等方面的广泛应用不断拓展。随着这一领域的迅速发展，我们意识到研究人员需要一个可供他们快速系统了解LLM基础论文的解读笔记仓库。

如今有许多LLM领域的研究论文，但为了获取全面的了解，研究人员往往需要花费大量时间筛选和阅读这些基础文献。LLM Research 的创立旨在为研究人员提供一个便捷的途径，集结LLM领域的经典论文，并提供论文的解读笔记供简单了解or深入学习这些论文。这种深度解析旨在帮助研究人员更好地理解论文的核心概念，并提供有深度的领域知识。

我们相信，通过LLM Research，研究人员可以更轻松地跟踪LLM领域的最新进展，拓展他们的知识边界。



## 项目规划

### a. 内容规划

我们的项目旨在创建一个系统全面的LLM基础论文解读笔记仓库，以支持对大型语言模型（LLM）领域的学术前沿感兴趣的研究人员。为了实现这一目标，我们已经组建了一个由5名成员组成的小组，专注于整理、深入解析和精读LLM领域的经典论文。想加入的同学们可以加负责人微信: linjh1118_nlp

每一篇精读笔记都将涵盖论文的核心思想、方法和关键贡献，旨在为研究人员提供深刻的理解。每篇笔记将分两个章节，第一个章节是TLDR版，其中将阐述文章的motivation、innovation、insight等核心思想以及核心代码，第二个章节则是全文精读版，这章节的行文逻辑按照原文的行文逻辑来，相当于对每段文章做一个summary，重点要放在methods和discussion，为读者提供一些深度解读。

具体内容见下: [经典论文列表](#经典论文列表)

### b. 人力规划

我们的项目将在接下来的三到四个月内进行。在这个时间框架内，我们小组将致力于每周产出5-7篇质量过关的论文笔记。这个周产出计划的目的是确保我们能够迅速而系统地覆盖LLM领域的广泛话题，并为研究人员提供及时的资源。同时，这也有助于确保我们的笔记在质量上经过仔细审查和审核。 此外，为了进一步确保笔记的质量，我们邀请了几位资深老师担任内容审核的角色。这些老师将负责审查、提供反馈，并确保每篇笔记符合标准。通过这一团队构成，我们有信心在规定时间内产出水平过关的经典论文笔记，为研究人员提供有价值的学术资源。



# 经典论文列表

- [Ch1. Parameter-Efficient Fine-Tuning](#ch1-parameter-efficient-fine-tuning)
  - [1. Low Rank Decomposition Method](#1-low-rank-decomposition-method)
  - [2. Continuous-Prompt Learning Method](#2-continuous-prompt-learning-method)
  - [3. Adapter Method](#3-adapter-method)
  - [4. Mixed Method](#4-mixed-method)
- [Ch2. Full Parameter Fine-Tuning](#ch2-full-parameter-fine-tuning)
  - [1. LOMO-series](#1-lomo-series)
- [Ch3. In-Context-Learning](#ch3-in-context-learning)
- [Ch4. Prompt Engineering](#ch4-prompt-engineering)
- [Ch5. LLM-based Agent](#ch5-llm-based-agent)
- [Ch6. LLM for Other Tasks](#ch6-llm-for-other-tasks)
  - [6.1 Relation Extraction](#61-relation-extraction)
  - [6.2 Graph Learning](#62-graph-learning)
  - [6.3 Knowledge Graph Reasoning](#63-knowledge-graph-reasoning)


## Ch1. Parameter-Efficient Fine-Tuning
目前还没有一个仓库有系统地整理“parameter-efficient-finetuning”领域论文。所以本仓库优先整理了这方面的论文。力求覆盖peft库中的基础微调方式。

### 1. Low Rank Decomposition Method

| Title                                                        | Date    | Publication | citation | Summary                                  | Notes   | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ---------------------------------------- | ------- | -------- |
| [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/pdf/2106.09685.pdf) | 2021-10 | arXiv       | 1555     |                                          | @林景豪 | 12.23    |
| [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning (AdaLoRA)](https://arxiv.org/pdf/2303.10512.pdf) | 2023-02 | ICLR        | 55       |                                          | @林景豪 | 12.23    |
| [LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307) | 2023-09 | arxiv       | 16       | [Lora_series_notes](Lora/Lora_series.md) | @林景豪 | 12.23    |
| [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/pdf/2305.14314.pdf) | 2023-05 | arxiv       | 224      |                                          | @胡锦琛 | 1.17     |
| [Orthogonal Subspace Learning for Language Model Continual Learning(o-lora)](https://arxiv.org/abs/2310.14152) | 2023-10 | arxiv       |          |                                          | @胡锦琛 | 1.27     |
| [S-LoRA: Serving Thousands of Concurrent LoRA Adapters](https://arxiv.org/abs/2311.03285) | 2023-11 | arxiv       |          |                                          | @胡锦琛 | 2.4      |

### 2. Continuous-Prompt Learning Method

| Title                                                        | Date    | Publication | citation | Summary | Notes   | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ------- | ------- | -------- |
| [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://arxiv.org/abs/2101.00190) | 2021-08 | ACL         | 1859     |         | @余绍缘 | 12.30    |
| [GPT Understands, Too (P-Tuning)](https://arxiv.org/abs/2103.10385) | 2021-03 | AI Open     | 307      |         | @余绍缘 | 1.6      |
| [The Power of Scale for Parameter-Efficient Prompt Tuning (Prompt-Tuning)](https://arxiv.org/abs/2104.08691) | 2021-04 | EMNLP       | 1683     |         | @余绍缘 | 1.13     |
| [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/abs/2110.07602) | 2021-10 | ACL         | 220      |         | @余绍缘 | 1.20     |
| [Late Prompt Tuning: A Late Prompt Could Be Better Than Many Prompts](https://arxiv.org/abs/2210.11292) | 2022-10 | EMNLP       | 6        |         | @余绍缘 | 1.27     |
| [Black-Box Tuning for Language-Model-as-a-Service](https://www.semanticscholar.org/paper/002c58077a1f1b296468b117230a1199e91f35c2) | 2022-06 | ICLR        | 100      |         | @余绍缘 | 2.4      |

### 3. Adapter Method

| Title                                                        | Date    | Publication | citation | Summary | Notes | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ------- | ----- | -------- |
| [Parameter-Efficient Transfer Learning for NLP (Adapter)](http://proceedings.mlr.press/v97/houlsby19a.html) | 2019-06 | ICML        | 1767     |         | @王淏 | 12.30    |
| [AdapterHub: A Framework for Adapting Transformers](https://arxiv.org/abs/2007.07779) | 2020-07 | EMNLP       |          |         | @王淏 | 1.6      |
|                                                              |         |             |          |         |       |          |

### 4. Mixed Method

| Title                                                        | Date     | Publication      | citation | Summary | Notes   | Deadline |
| ------------------------------------------------------------ | -------- | ---------------- | -------- | ------- | ------- | -------- |
| [UniPELT: A Unified Framework for Parameter-Efficient Language Model Tuning](https://arxiv.org/abs/2110.07577) | 2022-05  | ACL              | 79       |         | @林景豪 | 12.30    |
| [Towards a Unified View of Parameter-Efficient Transfer Learning](https://arxiv.org/abs/2110.04366) | 2022 -02 | ICLR (spotlight) | 385      |         | @林景豪 | 12.30    |
|                                                              |          |                  |          |         |         |          |



## Ch2. Full Parameter Fine-Tuning

### 1. LOMO-series
| Title                                                        | Date    | Publication | citation | Summary | Notes | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ------- | ----- | -------- |
| [Full Parameter Fine-tuning for Large Language Models with Limited Resources](https://arxiv.org/abs/2306.09782) | 2023-06 | arXiv       | 7        |         | @王淏 | 12.23    |
| [AdaLomo: Low-memory Optimization with Adaptive Learning Rate](https://arxiv.org/abs/2310.10195) | 2023-10 | arXiv       |          |         | @王淏 | 12.30    |
|                                                              |         |             |          |         |       |          |

## Ch3. In-Context-Learning

| Title                                                        | Date    | Publication | citation | Summary | Notes   | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ------- | ------- | -------- |
| [Chain of Thought Prompting Elicits Reasoning in Large Language Models](https://www.semanticscholar.org/paper/1b6e810ce0afd0dd093f789d2b2742d047e316d5) | 2023-01 | Nips2022    | 2141     |         | @袁鑫喆 | 12.30    |
| [Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them](https://www.semanticscholar.org/paper/663a41c866d49ce052801fbc88947d39764cad29) | 2022-10 | ACL2022     | 62       |         | @袁鑫喆 | 1.6      |
| [Automatic Chain of Thought Prompting in Large Language Models](https://www.semanticscholar.org/paper/90350aa626bed47b02d0c162462e5b0ca82be6b2) | 2022-10 | ICLR2022    | 200      |         | @袁鑫喆 | 1.13     |
| [Multimodal Chain-of-Thought Reasoning in Language Models](https://www.semanticscholar.org/paper/780a7f5e8ba9b4b451e3dfee1bcfb0f68aba5050) | 2023-02 | arxiv       | 100      |         | @袁鑫喆 | 1.20     |
|                                                              |         |             |          |         |         |          |

## Ch4. Prompt Engineering
| Title                                                        | Date    | Publication           | citation | Summary | Notes    | Deadline |
| ------------------------------------------------------------ | ------- | --------------------- | -------- | ------- | -------- | -------- |
| [Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing](https://www.semanticscholar.org/paper/28692beece311a90f5fa1ca2ec9d0c2ce293d069) | 2021-07 | ACM Computing Surveys | **1640** |         | ＠胡锦琛 | 12.30    |
| [Exploring Lottery Prompts for Pre-trained Language Models](https://www.semanticscholar.org/paper/a23d45f22e10173c58a5ee25e5b6c815829671d5) | 2023-05 | ACL                   | 1        |         | ＠胡锦琛 | 1.6      |
| Making Pre-trained Language Models Better Few-shot Learners  | 2021-06 | ACL                   | 1159     |         | ＠胡锦琛 | 1.13     |

## Ch5. LLM-based Agent
| Title                                                        | Date    | Publication | citation | Summary | Notes   | Deadline |
| ------------------------------------------------------------ | ------- | ----------- | -------- | ------- | ------- | -------- |
| [ToolLLM: Facilitating Large Language Models to Master 16000+ Real-world APIs](https://www.semanticscholar.org/paper/0bfc804e31eecfd77f45e4ee7f4d629fffdcd628) | 2023-10 | arxiv       | 53       |         | @王淏   | 1.6      |
| [AgentBench: Evaluating LLMs as Agents](https://www.semanticscholar.org/paper/5dbf93a68b7fda600521f046dea35ea8ba9e884f) | 2023-10 | arxiv       | 12       |         | @王淏   | 1.6      |
| [The Rise and Potential of Large Language Model Based Agents: A Survey](https://www.semanticscholar.org/paper/0c72450890a54b68d63baa99376131fda8f06cf9) | 2023-09 | arxiv       | 43       |         | @林景豪 | 1.6      |
| [Reflexion: Language Agents with Verbal Reinforcement Learning](https://www.semanticscholar.org/paper/0671fd553dd670a4e820553a974bc48040ba0819) | 2023-06 | arxiv       | **1640** |         | @林景豪 | 1.6      |
| [CAMEL: Communicative Agents for "Mind" Exploration of Large Scale Language Model Society](https://www.semanticscholar.org/paper/7ca954844bc1dd405bc43445b1c990e42d865095) | 2023-11 | Nips        | 61       |         | @林景豪 | 1.13     |
| Generative Agents: Interactive Simulacra of Human Behavior   | 2023-08 | arxiv       | 263      |         | @林景豪 | 1.13     |
| [Language Models can Solve Computer Tasks](https://www.semanticscholar.org/paper/9a75e23639bfcc3a51da57a3b682a984d1d8ac0b) | 2023-11 | Nips        | 62       |         | @王淏   | 1.13     |
| [ChatEval: Towards Better LLM-based Evaluators through Multi-Agent Debate](https://www.semanticscholar.org/paper/ec58a564fdda29e6a9a0a7bab5eeb4c290f716d7) | 2023-08 | arxiv       | 29       |         | @王淏   | 1.13     |
| [Improving Factuality and Reasoning in Language Models through Multiagent Debate](https://www.semanticscholar.org/paper/4780d0a027c5c5a8e01d7cf697f6296880ffc945) | 2023-05 | arxiv       | 75       |         | @王淏   | 1.20     |
| [Self-collaboration Code Generation via ChatGPT](https://www.semanticscholar.org/paper/ba2f935d2578fbf77ec1aa79e26e3db396771e38) | 2023-05 | arxiv       | 34       |         | @王淏   | 1.20     |
| Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf | 2023-09 | arxiv       | 10       |         | @林景豪 | 1.20     |
| [Describe, Explain, Plan and Select: Interactive Planning with Large Language Models Enables Open-World Multi-Task Agents](https://www.semanticscholar.org/paper/0935ce0adad57e1b24c50d793d46a407c3f563f3) | 2023-10 | Nips        | 79       |         | @林景豪 | 1.20     |





## Ch6. LLM for Other Tasks

### 6.1 Relation Extraction

| Title                                                                                                      | Date    | Publication | citation | Summary | Notes | Deadline |
| ---------------------------------------------------------------------------------------------------------- | ------- | ----------- | -------- | ------- | ----- | -------- |
| [Revisiting Relation Extraction in the era of Large Language Models](https://arxiv.org/pdf/2305.05003.pdf) | 2023-05 | ACL         | 14       |         | @王淏 | 1.20     |
|                                                                                                            |         |             |          |         |       |          |
|                                                                                                            |         |             |          |         |       |          |

### 6.2 Graph Learning

| Title                                                                                                                                       | Date    | Publication | citation | Summary | Notes   | Deadline |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ------- | ----------- | -------- | ------- | ------- | -------- |
| [G-Adapter: Towards Structure-Aware Parameter-Efficient Transfer Learning for Graph Transformer Networks](https://arxiv.org/abs/2305.10329) | 2023-05 | arXiv       |          |         | @袁鑫喆 | 1.20     |
|                                                                                                                                             |         |             |          |         |         |          |
|                                                                                                                                             |         |             |          |         |         |          |

### 6.3 Knowledge Graph Reasoning

| Title                                                                                                                         | Date    | Publication | citation | Summary | Notes   | Deadline |
| ----------------------------------------------------------------------------------------------------------------------------- | ------- | ----------- | -------- | ------- | ------- | -------- |
| [Making Large Language Models Perform Better in Knowledge Graph Completion (KoPA from ZJU)](https://arxiv.org/abs/2310.06671) | 2023-10 | arXiv       |          |         | @林景豪 | 1.20     |
|                                                                                                                               |         |             |          |         |         |          |
|                                                                                                                               |         |             |          |         |         |          |



# At last

**项目负责人**

- [林景豪-项目负责人&核心内容创作者](https://github.com/linjh1118)（东北大学研究生）
  微信: linjh1118_nlp
- [王淏-项目负责人&核心内容创作者](https://github.com/Charon-ops)（协和医学院医工所研究生）
  微信: Wandering_42

**核心贡献者**

- [余绍缘 核心内容创作者](https://github.com/shaoyuanyu) (吉林大学)
- [袁鑫喆 核心内容创作者](https://github.com) (吉林大学)
- [胡锦琛 核心内容创作者](https://github.com) (吉林大学)
- 吉林大学 车浩源，李昊天，段云娜老师们 核心内容创作者&审核者
- 东北大学 张富，程经纬老师们 核心内容创作者&审核者

**核心审查者**

1. 非常感谢导师们仔细审查了本仓库的所有笔记内容，
   感谢他们的大力支持，同时也感谢吉林大学机器人梦工厂和东北大学IDKE实验室的伙伴们的大力支持

2. 非常感谢datawhale组织的好大哥 **[谢文睿](https://github.com/Sm1les)**，**范晶晶**等对本项目的全程支持。

**How to contact me?**

If you have any questions or want to join us, please do not hesitate to contact me [linjh1118@mails.jlu.edu.cn](mailto:linjh1118@mails.jlu.edu.cn).

# 相关LLM学习仓库传送门
此外，我们整理了不少优秀的LLM方面的学习仓库，感谢他们的精彩开源贡献，在这里给出介绍和传送门。

-  [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM)仓库由[Xin Cheng](https://github.com/Hannibal046)等人创建，其中汇总了LLM中各方向的高质量论文，同时也包含针对LLM训练，部署应用，入门博客教程等各种资料的地址。
-  [ICL_PaperList](https://github.com/dqxiu/ICL_PaperList)仓库由[Qingxiu Dong](https://github.com/dqxiu/ICL_PaperList)等人创建，其中汇总了LLM子方向ICL的高质量论文，同时也孵化出了一篇优秀的综述。
- [邹雨衡](https://github.com/logan-zou),  [长琴](https://yam.gift/),  [玉琳](https://github.com/Sophia-Huang)和众多datawhale开源贡献者一起创作了[datawhalechina/prompt-engineering-for-developers](https://github.com/datawhalechina/prompt-engineering-for-developers)，详实地介绍了prompt engineering，如何用chatgpt和langchain搭建LLM应用，如何使用 Gradio 搭建生成式 AI 应用等内容。非常推荐一学~
- [邹雨衡](https://github.com/logan-zou)的[动手写LLM应用开发](logan-zou/Tutorial_for_developing_LLM_application)是一个面向小白开发者的大模型应用开发教程，旨在结合个人知识库助手项目，通过一个课程完成大模型开发的重点入门。此教程不仅包含了很多LLM开发的实战知识，其对LLM各方面基础知识也进行全面介绍。非常推荐一学~
- [长琴](https://yam.gift/) 等人的[datawhalechina/hugging-llm](https://github.com/datawhalechina/hugging-llm)详细地介绍了ChatGPT原理、使用和应用。读者学习了之后，即可熟练地编写相应代码来调用openai的api进而完成NLP各种下游任务。
- [陈安东](https://github.com/andongBlue)和[张帆](https://github.com/zhangfanTJU)的[datawhalechina/so-large-lm](https://github.com/datawhalechina/so-large-l)对大模型做出了一个详细的综述，介绍了大模型的技术内容(数据准备、模型构建、训练策略到模型评估与改进等方面)，也介绍了大模型的伦理内容(安全、隐私、环境和法律道德等方面)。非常推荐一学。
- [不要葱姜蒜](https://github.com/KMnO4-zx)的[self-llm](https://github.com/datawhalechina/self-llm/tree/master)针对各类开源大模型提供包括环境配置、本地部署、高效微调等技能在内的全流程指导，简化开源大模型的部署、使用和应用流程，让更多的普通学生、研究者更好地使用开源大模型，帮助开源、自由的大模型更快融入到普通学习者的生活中。通过这个项目，读者可以本地部署大模型(Chatglm3, Yi, Qwen, Baichuan)等实现一些有趣的LLM案例~ 非常推荐一学~

