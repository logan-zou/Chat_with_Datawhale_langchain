# smoothly-vslam

- **项目简介** 

  👋  **欢迎来到VSLAM的世界**<br />SLAM是一个与传感器紧密联系的系统，VSLAM使用的传感器就是摄像头。处理摄像头数据需要理解相机成像的过程，这是一个从现实世界到计算机能处理的数据的映射过程。通过这节，你会知道相机的成像模型及映射过程的几个坐标系。与之相关的是相机的畸变及内参标定。这对应于第一章。<br />观测数据所处坐标系为传感器坐标系，为局部观测，我们需要将局部观测转换到全局观测上，这就涉及坐标系间转换。将传感器坐标系观测转换到载体坐标系需要通过外参，计算载体坐标系在世界坐标系下坐标需要用到三维空间中刚体运动变换。这两部分分别对应第二章与第三章。<br />通过上面三部分，基本就可以知道VSLAM的前端工作的一个背景了。可以想象VSLAM系统是在一个载体上搭载着摄像头，在未知环境中不断移动，对环境及自身位姿进行同时估计。那么什么是VSLAM？这块会在第四章进行介绍。<br />通过第四章，我们知道目前成熟的VSLAM框架主要包含前端，后端，回环检测及建图四个模块，这会在后续章节依次介绍。<br />前端为视觉里程计，即VO。我们着重介绍目前使用的较多的特征点法VO，也就是间接法。传统特征点法依赖人工设计的视觉特征，这块会在第五章进行介绍。<br />基于特征点的提取与匹配，我们可以对相机的位姿及特征点的三维空间位姿进行估计，这部分主要分为两个过程，即初始化过程及帧间位移估计。初始化需要确定三维空间点坐标，世界坐标系及尺度，比较复杂，在初始化完成后，就可以通过特征匹配，比较轻松得获得相机帧间位移。这两个过程会在第六章及第七章进行介绍。<br />介绍完视觉前端，接下来是视觉后端，按照使用不同技术，分为基于滤波的方法与非线性优化的方法。这两部分对应于第八章及第九章。<br />然后是回环检测模块，这部分会在第十章进行讲解。<br />VSLAM最后一个重要模块建图对应于第十一章，这也是主教程最后一个章节。<br />如果学有余力，可以看第十二章实践章节，亲自设计一个VSLAM系统。如果完成这个章节，你会获得很大的成就感，对于后面工程应用会有很大帮助。<br />最后就是进度，每天看一点就行。学到很多东西的秘诀，就是每次不要看太多。\

  教程博客在线阅读地址一：[smoothly-vslam](https://www.yuque.com/u1507140/vslam-hmh)

<a name="lKFny"></a>
### 推荐书籍
VSLAM属于一个交叉系统学科，包含很多方向的内容，如多视图几何，状态估计，优化等等，以下是部分推荐书籍：<br />1.多视图几何

- 《Multiple View Geometry in Computer Vision 》
- [《计算机视觉中的数学方法》](http://in.ruc.edu.cn/wp-content/uploads/2021/01/Maths-in-3D-computer-vision.pdf)

2.刚体运动

- 李群和李代数: [Quaternion kinematics for the error-state Kalman filter  ](http://www.iri.upc.edu/people/jsola/JoanSola/objectes/notes/kinematics.pdf)
- 《机器人学中的状态估计》原作者蒂莫西.D.巴富特，译者高翔。

3.VSLAM介绍

- 《视觉SLAM十四讲:从理论到实践》
- [高翔博士的博客](https://www.cnblogs.com/gaoxiang12/p/3695962.html)
- - D. Scaramuzza, F. Fraundorfer, "Visual Odometry: Part I - The First 30 Years and Fundamentals IEEE Robotics and Automation Magazine", Volume 18, issue 4, 2011.
- - F. Fraundorfer and D. Scaramuzza, "Visual Odometry : Part II: Matching, Robustness, Optimization, and Applications," in IEEE Robotics & Automation Magazine, vol. 19, no. 2, pp. 78-90, June 2012.

4.概率论

- 《概率机器人》

5.优化理论

- [数值最优化（第二版）(美)乔治·劳斯特(Jorge Nocedal)](https://www.math.uci.edu/~qnie/Publications/NumericalOptimization.pdf)
- 凸优化：[Convex Optimization ](https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf)
- 凸优化：[Introductory Lectures on Convex Programming](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.693.855&rep=rep1&type=pdf)
- [g2o](http://ais.informatik.uni-freiburg.de/publications/papers/kuemmerle11icra.pdf)
- 《机器人感知：因子图在SLAM中的应用》（gtsam作者，佐治亚理工教授 Frank Dellaert写的）

优化理论进阶

- Nolinear Programming

6.一些工具

- ubuntu, cmake, [bash](https://www.zhihu.com/search?q=bash&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra=%7B%22sourceType%22%3A%22answer%22%2C%22sourceId%22%3A145219653%7D), vim, qt(optional).
- OpenCV install, read the opencv reference manual and tutorial.
-  ros install： [ROS/Installation - ROS Wiki](https://link.zhihu.com/?target=http%3A//wiki.ros.org/ROS/Installation)
- ros [tutorial](https://www.zhihu.com/search?q=tutorial&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra=%7B%22sourceType%22%3A%22answer%22%2C%22sourceId%22%3A145219653%7D): [ROS/Tutorials - ROS Wiki](https://link.zhihu.com/?target=http%3A//wiki.ros.org/ROS/Tutorials) \

如果你想对本教程做贡献，请邮件联系：530019431@qq.com

Finally, hope you enjoy it！

  
- **项目内容目录** \
**0.前言** \
**1.一幅图像的诞生：相机投影及相机畸变** \
**2.差异与统一：坐标系变换与外参标定** \
**3.描述状态不简单：三维空间刚体运动** \
**4.也见森林：视觉SLAM简介** \
**5.以不变应万变：前端-视觉里程计之特征点** \
**6.换一个视角看世界：前端视觉里程计之对极几何** \
**7.积硅步以至千里：前端-视觉里程计之相对位姿估计** \
**8.在不确定中寻找确定：后端之卡尔曼滤波** \
**9.每次更好，就是最好：后端之非线性优化** \
**10.又回到曾经的地点：回环检测** \
**11.终识庐山真面目：建图** \
**12.实践是检验真理的唯一标准：设计VSLAM系统** 

 - **项目在线阅读地址**\
  https://www.yuque.com/u1507140/vslam-hmh

## Roadmap

这里列一些还需要完善的部分
### 1.对各章节内容的进一步的完善
补充各章节的基础内容，从背景发展到具体的算法原理的进一步充实
比如，对第八章，卡尔曼滤波可以有如下的进一步完善
- 1.贝叶斯滤波的补充
- 2.其他滤波的介绍

### 2.内容的进阶，不仅限于VSLAM内容
- 1.SLAM更一般的理论基础，如可观性，退化场景分析
- 2.SLAM应用场景等等


**当前教程为VSLAM基础教程，涉及VSLAM背景知识及基础算法原理，对更深入的部分，计划后续开一个进阶教程进行讲解。**

## 参与贡献

- 如果你想参与到项目中来欢迎查看项目的 [Issue]() 查看没有被分配的任务。
- 如果你发现了一些问题，欢迎在 [Issue]() 中进行反馈🐛。
- 如果你对本项目感兴趣想要参与进来可以通过 [Discussion]() 进行交流💬。

如果你对 Datawhale 很感兴趣并想要发起一个新的项目，欢迎查看 [Datawhale 贡献指南](https://github.com/datawhalechina/DOPMC#%E4%B8%BA-datawhale-%E5%81%9A%E5%87%BA%E8%B4%A1%E7%8C%AE)。


## 贡献者名单

| 姓名 | 职责 | 简介 | 联系方式|
| :----| :---- | :---- |:---- |
| 胡明豪 | 项目负责人，教程初版贡献者 | DataWhale成员，VSLAM算法工程师 |530019431@qq.com|
| 王洲烽 | 第1，2章贡献者 | DataWhale成员，国防科技大学准研究生 | wangzhoufeng7346@gmail.com |
| 乔建森 | 第3，5，8，9章贡献者| 中国航天科工三院-算法工程师 | 2719008838@qq.com |
| 林俊强 | 第5章贡献者| 算法工程师 | hayasijq@gmail.com |



## 关注我们

<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "180" height = "180">
</div>



## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。

