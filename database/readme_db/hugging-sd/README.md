<div align="center">
<img  src="./resource/huggingsd.png" width="1000">
</div>

<p align="center">
    <!-- license badge -->
    <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" />
    </a>
</p>

### 项目简介

受到[HuggingLLM](https://github.com/datawhalechina/hugging-llm)项目的启发，本项将介绍以stable-diffusion为代表的视觉生成大模型的原理、使用和应用，降低使用门槛，让更多感兴趣的非专业人士能够无障碍使用SD创造价值。

### 立项理由

以stable-diffusion为代表的视觉生成大模型正在深刻改变视觉领域中的上下游任务（包括二维、三维、视频）。且正在改变许多行业，比如绘画、3D建模、影视、游戏等等。我们将借助该项目让更多人了解并使用视觉生成大模型，尤其是对此感兴趣、想利用相关技术做一些新产品或应用的朋友。希望新的技术能够促进行业更快更好发展，提高人们工作效率和生活质量。AI for humans!

### 项目受众

项目适合以下人员：

- 学生。希望通过学习相关技术，或是开发新应用，或是入门视觉生成式大模型，或是结合其他行业做AI for science的研究等。
- 相关或非相关行业从业者。对stable-diffusion或视觉生成大模型感兴趣，希望在实际中运用该技术创造提供新的服务或解决已有问题。

项目不适合以下人员：

- 研究底层算法细节，比如DDPM数学推导、讨论SDS / SJC VSD等。
- 对其他技术细节感兴趣。

### 项目亮点

聚焦于如何使用stable-diffusion API创造新的功能和应用（二维和三维）。
了解相关算法原理以更便捷高效使用。
提供示例代码和使用流程。

### 项目规划【内容持续更新中，欢迎关注～】

**二维生成**
- 1 stable-diffusion原理简介
    - 1.1 视觉生成方法
    - 1.2 [DDPM算法](./content/1-2%20DDPM算法.ipynb)
- 2 stable-diffusion使用指南
    - 2.1 提示词
    - 2.2 文生图
    - 2.3 [图生图](./content/2-3%20图生图.ipynb)
    - 2.4 生成优化
      - 2.4.1 [Textual Inversion](./content/2-4-1%20Textural%20Inversion.ipynb)
      - 2.4.2 [DreamBooth](./content/2-4-2%20DreamBooth.ipynb)
      - 2.4.3 [LoRA](./content/2-4-3%20LoRA.ipynb)
      - 2.4.4 ControlNet
    - 2.5 插件与工具
    - 2.6 [sdxl1.0与应用](./content/2-6%20sdxl1.0与应用.ipynb)


**三维生成**
- 3 三维生成原理
    - 3.1 [背景及应用](./content/3-1%20背景及应用.md)
    - 3.2 [NeRF神经辐射场](./content/3-2%20NeRF神经辐射场.ipynb)
    - 3.3 [文生3D](./content/3-3%20文生3D.md)
    - 3.4 可控3D生成
- 4 三维视觉应用
    - 4.1 blender入门
    - 4.2 3D重建与打印

**视频生成**
- 5 视频编辑
    - 5.1 风格迁移
    - 5.2 场景编辑
- 6 视频生成
    - 6.1 文生视频
    - 6.2 图生视频

**技术局限与未来发展**
- 7 目前局限
  - 二维生成：版权等
  - 三维生成：质量有待提升、生成时间长、渲染速度慢等
  - 视频生成：稳定性、连续性等
- 8 未来发展
  - 8.1 [社区生态](./content/8-1%20社区生态.md)
  - 8.2 行业应用
      - 二维场景：营销作图、游戏作画、美图工具等
      - 三维场景：游戏、数字人、电影、虚拟资产、vision pro内容等
      - 视频场景：抖音、b站、直播等

### 贡献者
<table border="0" >
  <tbody>
    <tr align="center" >
      <td>
         <a href="https://github.com/xjli360"><img width="70" height="70" src="https://github.com/xjli360.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/xjli360">Xiaojie Li</a> 
         <p>项目负责人<br>清华大学硕士</p>
      </td>
      <td>
         <a href="https://github.com/guanidine"><img width="70" height="70" src="https://github.com/guanidine.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/guanidine">Letian Zhang</a>
         <p>主要贡献者<br>清华大学硕士</p>
      </td>
      <td>
         <a href="https://github.com/joyenjoye"><img width="70" height="70" src="https://github.com/joyenjoye.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/joyenjoye">joye</a> 
        <p>主要贡献者<br>Data Scientist</p>
      </td>
      <td>
         <a href="https://github.com/KashiwaByte"><img width="70" height="70" src="https://github.com/KashiwaByte.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/KashiwaByte">Bote Huang</a>
         <p>主要贡献者<br>西安电子科技大学本科</p>
      </td>
    </tr>
  </tbody>
</table>


<table border="0">
  <tbody>
    <tr align="center" >
      <td>
         <a href="https://github.com/Fantastic121380"><img width="70" height="70" src="https://github.com/Fantastic121380.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/Fantastic121380">Di Yu</a>
         <p>主要贡献者<br>清华大学硕士</p>
      </td>
      <td>
         <a href="https://github.com/flawzhang"><img width="70" height="70" src="https://github.com/flawzhang.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/flawzhang">Qiang Zhang</a>
         <p>主要贡献者<br>清华大学硕士</p>
      </td>
      <td>
         <a href="https://github.com/mxztflow"><img width="70" height="70" src="https://github.com/mxztflow.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/mxztflow">Xiaozhuang Ma</a>
         <p>主要贡献者<br>西安交通大学硕士</p>
      </td>
      <td>
         <a href="https://github.com/QJieWang"><img width="70" height="70" src="https://github.com/QJieWang.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/QJieWang">Qingjie Wang</a>
         <p>主要贡献者<br>中国科学技术大学</p>
      </td>
    </tr>
  </tbody>
</table>

### 致谢
特别感谢 [Sm1les](https://github.com/Sm1les)对本项目的帮助与支持。
感谢[Tango](https://github.com/it-worker-club)对2-2章节提供的部分帮助；感谢[AnSuZeaT](https://github.com/AnSuZeaT)对6-1章节提供的部分帮助。

### 关注我们

<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="resource/qrcode.jpeg" width = "180" height = "180">
</div>
&emsp;&emsp;Datawhale，一个专注于AI领域的学习圈子。初衷是for the learner，和学习者一起成长。目前加入学习社群的人数已经数千人，组织了机器学习，深度学习，数据分析，数据挖掘，爬虫，编程，统计学，Mysql，数据竞赛等多个领域的内容学习，微信搜索公众号Datawhale可以加入我们。

### LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。
