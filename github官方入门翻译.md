#Github 官方入门教程（中文版）
** Hello World **工程是计算机编程学习的传统。它帮助你通过一个简单的练习入门一项新的编程技能。下面开始学习使用GitHub。

** 你将要学习到： **

* 创建并使用仓库（repository）
* 创建并管理一个新的分支（branch）
* 改变一个文件并通过创建一个提交（commit）讲该改动推到（push）GitHub上
* 开启、合并一个合并请求（pull request）

##GitHub是什么？
GitHub是一个用户代码版本控制和团队写作的代码托管平台。它使你和其他人无论身处何处都可以为同一项目一同工作。

本使用说明教将介绍GitHub最基本的概念，例如：仓库（repositories）、分支（branched）、提交（commits）、合并请求（pull request）。你将创建你自己的Hello World仓库，并且学习GitHub的Pull Request工作流程，它是一个非常流行的创建、检查代码的流程。

###无需编程
完成本说明教程所需条件为：1.一个GitHub账号。2.一台联网的电脑。你不需要会写代码，不需要会使用命令行，甚至不需要安装Git（Git是一个版本控制软件，GitHub已经内置）
> Tip:将本说明教程置于单独的浏览器页面，这样就可以一边参照说明教程，一边在GitHub上进行操作。

##第一步：创建仓库
仓库（repository）通常用于组织一个单独的工程项目。仓库包含文件夹、文件、图片、视频、表格、数据集等，任何工程中需要的东西。我们建议仓库中包含一个README文件或者一个介绍本项目的说明文件。GitHub使你可以很方便的在创建仓库的同时添加这样的说明文件。同时，也提供了证书文件（license file）的添加。

你的** Hello World **仓库可以用来记录想法，积累源代码，甚至可以用来跟其他人分享，讨论。

###创建一个新的仓库
1. 点击首页右上方，头像左边的“+”，选择新建仓库（ ** New repository **）。
2. 给仓库命名为hello-world 。
3. 写一个简短的说明。
4. 勾选初始化项目的说明文件README（** Initialize this repository with a README **) 。
![](https://guides.github.com/activities/hello-world/create-new-repo.png)

点击创建仓库（** Create repository **）

##第二步：创建分支
分支的作用是使得在同一时间操作仓库的不同版本成为可能。

默认情况下，一个仓库会有一个名为master的分支，该分支通常作为限定分支存在。我们在其他分支上进行实验，编辑其他分支，然后再将这些产生变更的分支提交到master分支。
当你在master分支的基础上创建一个分支的时候，相当于在这个时间点为master分支制作了一个备份或者快照。当其他人在master上进行了变更操作，你可以通过pull操作更新这些变更。

这个过程如下图所示：
* master分支
* 一个名为feature的新分支（因为我们正在这个分支上做“特征工作”）
* 这个过程中，先创建feature分支然后再将该分支合并到master分支

![](https://guides.github.com/activities/hello-world/branching.png)

你是否保存了一个文件的不同版本？就像这样：
* story.txt
* story-joe-edit.txt
* story-joe-edit-reviewd.txt

分支在GitHub的仓库中起到的作用跟上边的情况很相似。

在GitHub上，开发者，作者，设计师能够用分支进行bug修复操作，而不会破坏master（生产）分支。当一个变更确认完成之后，可以将这个分支合并（merge）到master分支。

###创建一个新的分支
1. 进入你的新hello-world仓库。
2. 点击文件列表上方名为Branch: master的下拉箭头。
3. 输入新建的分支名，这里取名为readme-edits 。
4. 点击蓝色提示，Create branch，或者用键盘回车键进行确认。

![](https://guides.github.com/activities/hello-world/readme-edits.gif)

现在有两个分支，master和readme-edits。到目前为止他们看起来很像，但也仅仅是到目前为止。接下来会在新建分支上进行改动。

##第三步：在分支上进行改动，并提交改动

非常棒！现在我们即将对新建的readme-edits分支进行代码审查，这个分支是master的复制版本。让我们进行一些改动。

在GitHub上