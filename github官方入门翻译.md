#Github 官方入门教程（中文版）

>官方英文版地址：https://guides.github.com/activities/hello-world/

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
> 提示:将本说明教程置于单独的浏览器页面，这样就可以一边参照说明教程，一边在GitHub上进行操作。

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

在GitHub上,保存的变更叫做提交（commit），每一个提交都有一个相关的提交信息（commit message），这些提交信息对本次变更进行了解释。提交信息能够记录所有的变更，因此其他维护人员能够理解你已经做了哪些工作，以及为什么这么做。

###进行变更和提交变更的步骤

1. 打开README.md文件。
2. 点击铅笔按钮，该按钮在右上角删除键旁边。
3. 在文件中介绍一下你自己。
4. 写一个提交信息，对你的变更进行描述。
5. 点击提交变更（** Commit changes **）绿色按钮。

![](https://guides.github.com/activities/hello-world/commit.png)

这些变更只会出现在readme-edits分支的README文件上，因此这个分支的内容跟master分支的内容不同了。

## 第四步：发起一个合并请求

在经过了一个非常棒的编辑之后，master分支之下的readme-edits分支上已经发生了变更，现在可以发起一个合并请求了。

合并请求（Pull Requests）是GitHub上协作的核心内容。当你发起一个合并请求的时候，你提出了你的变更并且请求其他人进行复查并引入你的变更，如果没有问题，这些变更将会被合并到他们的分支上。这些变更，增加内容，删减内容都会呈现绿色或者红色进行区分。

一旦你做了一个提交，就可以发起一个合并请求并且开始讨论，即使代码没有完全完成。

通过利用github的@功能，你可以在合并请求中特别提醒某人或者某个团队，从而获得他们的反馈，无论你们近在咫尺还是远在天边。

你甚至可以在自己的仓库中向自己发起合并请求，从而熟悉GitHub的工作流程，使得以后可以更好应对大型团队合作。

### 为README文件的变更发起一个合并请求

1. 点击Pull Request栏目，填写合并请求页的信息，然后点击绿色pull request按钮。
![](https://guides.github.com/activities/hello-world/pr-tab.gif)
2. 在例程比较栏中选择提交合并请求的分支readme-edits，去跟master分支进行比较。
![](https://guides.github.com/activities/hello-world/pick-branch.png)
3. 在对比页中仔细检查这些变动，确保这些变动是你要提交的。
![](https://guides.github.com/activities/hello-world/diff.png)
4. 当检查完毕，确认这些变动是你想要提交的，点击大的绿色的创建合并请求（Create Pull Request）按钮。
![](https://guides.github.com/activities/hello-world/create-pr.png)
5. 为合并请求命名并进行简要描述。然后点击创建合并请求（** Create pull request **）按钮。
![](https://guides.github.com/activities/hello-world/pr-form.png)

## 第五步：合并请求
最后，是时候把readme-edits分支的变更合并到master 分支了。

1. 点击绿色合并请求（Merge pull request）按钮，将变更合并到master分支。
![](https://guides.github.com/activities/hello-world/merge-button.png)
2. 点击确认合并（ Confirm merge.）。
3. 删除已经合并的分支，因为变更已经被融合到master分支中了。删除按钮在紫色框中。
![](https://guides.github.com/activities/hello-world/delete-button.png)


## 完成！

在学习完成这个使用说明之后，你已经学习如何创建工程，并在GitHub上发起一个合并请求（pull request）。
总一下，你已经学习了：
* 创建一个开源仓库
* 创建并管理一个新的分支
* 对一个文件进行变动，并向GitHub提交这些变更。
* 发起并合并一个合并请求（Pull Request）

查看一下你的GitHub资料页，你会看到你的新贡献方块。

关于更多合并请求（Pull Requests）的知识，我们推荐你阅读[GitHub工作流指导手册](https://guides.github.com/introduction/flow/) ,你也可以访问 [GitHub Explore](https://github.com/explore)对开源项目进行深入了解。

>提示:查看我们的其他[说明文档](https://guides.github.com/),[油管频道](https://www.youtube.com/githubguides),[按需训练](https://services.github.com/on-demand/),从而了解更多GitHub入门知识。

译者注：能力有限，难免纰漏，如有错误，欢迎指正，我的联系方式：zykstand@foxmail.com
