# faster-git

课程内容：

1. [第一章 Git简介](lecture01/README.md)
1. [第二章 Git基础命令](lecture02/README.md)
1. [第三章 Git分支管理](lecture03/README.md)
1. [第四章 Git工具](lecture04/README.md)
1. [第五章 Git内部原理](lecture05/README.md)
1. [第六章 GitFlow工作流实战](lecture06/README.md)
1. [第七章 Git提交规范](lecture07/README.md)
1. [第八章 Github/Gitee使用说明](lecture08/README.md)
1. [第九章 Git可视化工具下载](lecture09/README.md)
1. [第十章 Git团队协作以及合并时的diff工具](lecture10/README.md)

课程安排：
| 任务信息                                                    |
|-------------------------------------------------------------|
| Task01：Git基础：第一、二章（2天）                          |
| Task02：Git分支管理及工具使用：第三、四章（2天）            |
| Task03：Git内部原理及工作流实战：第五、六章（3天）          |
| Task04：Git提交规范及Github/Gitee的使用：第七、八章（3天）  |
| Task05：Git可视化工具下载和团队协作：第九、十章（3天）      |

课程贡献人员：（排名不分先后，按章节顺序排序）
| 成员&nbsp; | 个人简介                                            | 负责章节|
| --------------- | --------------------------------------------------- |-------|
|   牛志康   | Datawhale成员，西安电子科技大学本科生 | lecture01，lecture03|
|朱松青| Datawhale成员，上海交通大学研究生|lecture02|
|徐祥军|在职，互联网金融、后端开发|lecture04|
|李碧涵|Datawhale成员，在职|lecture05|
|   宋泽山   | Datawhale成员，算法开发 | lecture06|
|王晓亮|Datawhale成员，在职|lecture07|
|张翔宇|华东师范大学研究生|lecture08|
|    沈豪    | Datawhale成员，复旦大学网安博士在读 |lecture09|
|   夏峻   | Datawhale成员，上海交通大学研究生  |lecture10|

# Contributing

主分支为`main`
## Workflow

关于本项目中出现的问题或者其他补充材料，我们鼓励大家提出pr和issue，我们将在短时间内进行解答。本项目使用`Forking`工作流，具体参考[atlassian文档](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)

大致步骤如下：

1. 在GitHub上Fork本仓库
1. Clone Fork后的个人仓库
1. 设置`upstream`仓库地址，并禁用`push`
1. 使用分支开发，课程分支名为`lecture{#NO}`，`#NO`保持两位，如`lecture07`，对应课程目录
1. PR之前保持与原始仓库的同步，之后发起PR请求

命令示例：

```shell
# fork
# clone
git clone git@github.com:USERNAME/faster-git.git

# set upstream
git remote add upstream git@github.com:datawhalechina/faster-git.git
# disable upstream push
git remote set-url --push upstream DISABLE
# verify
git remote -v
# some sample output:
# origin	git@github.com:tomowang/faster-git.git (fetch)
# origin	git@github.com:tomowang/faster-git.git (push)
# upstream	git@github.com:datawhalechina/faster-git.git (fetch)
# upstream	DISABLE (push)

# do your work
git checkout -b lecture07
# edit and commit and push your changes
git push -u origin lecture07

# keep your fork up to date
## fetch upstream main and merge with forked main branch
git fetch upstream
git checkout main
git merge upstream/main
## rebase brach and force push
git checkout lecture07
git rebase main
git push -f
```

## Commit Message

提交信息使用如下格式：`<type>: <short summary>`

```
<type>: <short summary>
  │            │
  │            └─⫸ Summary in present tense. Not capitalized. No period at the end.
  │
  └─⫸ Commit Type: lecture{#NO}|others
```

`others`包括非课程相关的改动，如本`README.md`中的变动，`.gitignore`的调整等。

## 关注我们
<div align=center><img src="https://raw.githubusercontent.com/datawhalechina/easy-rl/master/docs/res/qrcode.jpeg" width = "250" height = "270" alt="Datawhale是一个专注AI领域的开源组织，以“for the learner，和学习者一起成长”为愿景，构建对学习者最有价值的开源学习社区。关注我们，一起学习成长。"></div>

## LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。

