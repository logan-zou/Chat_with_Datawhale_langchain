 [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl-book)](https://github.com/datawhalechina/joyrl-book/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl-book)](https://github.com/datawhalechina/joyrl-book/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl-book)](https://github.com/datawhalechina/joyrl-book/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl-book)](https://github.com/datawhalechina/joyrl-book/blob/master/LICENSE)
# JoyRL Book

继[《蘑菇书》](https://github.com/datawhalechina/easy-rl)之后，我们对于想要更多地深入了解强化学习实践的读者准备了一套全新的教程，全书主要基于笔者“不那么丰富可是也有一点咯”的实践经验，帮助读者快速入门强化学习的代码实践，并辅以一套开源代码框架`JoyRL`，便于读者适应业界应用研究风格的代码。

与《蘑菇书》不同，本教程侧重对强化学习核心理论的提点和串联，以及对于强化学习代码实践的指导，尽可能还原原论文的主要思想，而不是对于理论的详细讲解。因此，《蘑菇书》适合适合细嚼慢咽的读者，而本教程则适合具有一定编程基础且希望快速进入实践应用的读者。

## 关于`JoyRL`

[JoyRL](https://github.com/datawhalechina/joyrl)旨在建立一套帮助初学者或交叉学科研究者快速入门强化学习的代码生态。它以`PiP`包的形式开发开源框架，英文注释，会比离线版更加集成，更加高效，并且会去掉一些实际并不常用的基础算法，例如`Q-learning`等等，适合需要大规模环境应用的读者进阶使用。

此外，本书中的演示代码会在以`Jupyter Notebook`的形式呈现，具体在[notebooks](./notebooks)文件夹中。

## 在线阅读(内容实时更新)

地址：https://datawhalechina.github.io/joyrl-book/

## 内容导航

|               章节                | 关键内容 |
| :-------------------------------: | :--: |
|       [第一章 绪论](https://datawhalechina.github.io/joyrl-book/#/ch1/main)       |  |
| [第二章 马尔可夫决策过程](https://datawhalechina.github.io/joyrl-book/#/ch2/main) | 马尔可夫决策过程、状态转移矩阵 |
|     [第三章 动态规划](https://datawhalechina.github.io/joyrl-book/#/ch3/main)     | 贝尔曼方程、策略迭代、价值迭代 |
|    [第四章 免模型预测](https://datawhalechina.github.io/joyrl-book/#/ch4/main)    | 蒙特卡洛、时序差分 |
|    [第五章 免模型控制](https://datawhalechina.github.io/joyrl-book/#/ch5/main)    | Q-learning 算法、Sarsa 算法 |
| [第六章 深度学习基础](https://datawhalechina.github.io/joyrl-book/#/ch6/main) | 神经网络、梯度下降 |
| [第七章 DQN算法](https://datawhalechina.github.io/joyrl-book/#/ch7/main) | DQN 算法、目标网络、经验回放 |
| [第八章 DQN算法进阶](https://datawhalechina.github.io/joyrl-book/#/ch8/main) | Double DQN、Dueling DQN、PER DQN |
| [第九章 策略梯度](https://datawhalechina.github.io/joyrl-book/#/ch9/main) | 随机性策略、REINFORCE |
| [第十章 Actor-Critic算法](https://datawhalechina.github.io/joyrl-book/#/ch10/main) | A2C、A3C |
| [第十一章 DDPG算法](https://datawhalechina.github.io/joyrl-book/#/ch11/main) | DDPG、TD3 |
| [第十二章 PPO算法](https://datawhalechina.github.io/joyrl-book/#/ch12/main) | 重要性采样、PPO |
| [第十三章 SAC算法](https://datawhalechina.github.io/joyrl-book/#/ch13/main) | 最大熵强化学习、Soft Q、SAC |
| [JoyRL 中文文档](https://datawhalechina.github.io/joyrl-book/#/joyrl_docs/main) |  |
| [练习题解答](https://datawhalechina.github.io/joyrl-book/#/appendix/main) |  |

## 主要贡献者

<table border="0">
  <tbody>
    <tr align="center" >
        <td>
         <a href="https://github.com/JohnJim0816"><img width="70" height="70" src="https://github.com/JohnJim0816.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/JohnJim0816">John Jim</a>
         <p>教程设计与算法实战<br> 北京大学硕士 </p>
        </td>
        <td>
            <a href="https://github.com/qiwang067"><img width="70" height="70" src="https://github.com/qiwang067.png?s=40" alt="pic"></a><br>
            <a href="https://github.com/qiwang067">Qi Wang</a> 
            <p>教程设计<br> 上海交通大学博士生<br> 中国科学院大学硕士</p>
        </td>
        <td>
            <a href="https://github.com/yyysjz1997"><img width="70" height="70" src="https://github.com/yyysjz1997.png?s=40" alt="pic"></a><br>
            <a href="https://github.com/yyysjz1997">Yiyuan Yang</a> 
            <p>教程设计 <br> 牛津大学博士生<br> 清华大学硕士</p>
        </td>
    </tr>
  </tbody>
</table>

## 特别感谢

* 协助编辑与校对。[@AzulaFire](https://github.com/limafang)

## 关注我们

扫描下方二维码关注公众号：Datawhale，回复关键词“强化学习”，即可加入“EasyRL & JoyRL 读者交流群”
<div align=center><img src="https://raw.githubusercontent.com/datawhalechina/easy-rl/master/docs/res/qrcode.jpeg" width = "250" height = "270" alt="Datawhale是一个专注AI领域的开源组织，以“for the learner，和学习者一起成长”为愿景，构建对学习者最有价值的开源学习社区。关注我们，一起学习成长。"></div>