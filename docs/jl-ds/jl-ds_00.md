# 前言

*数据科学家：21 世纪最性感的职业*，《哈佛商业评论》。那么，为什么选择 Julia？作为一种高级语言，拥有庞大的科学社区，并且性能可与 C 相媲美，Julia 被誉为数据科学的最佳语言。使用 Julia，我们可以创建统计模型、高效的机器学习系统，并生成美观、引人注目的可视化。

# 本书内容

第一章，*基础知识 - Julia 环境*，解释了如何设置 Julia 的环境（命令行（REPL）和 Jupyter Notebook），并介绍了 Julia 的生态系统，为什么 Julia 是特别的，以及包管理。它还介绍了并行处理和多重派发，并解释了 Julia 如何适用于数据科学。

第二章，*数据清理*，解释了数据准备的必要性和过程，也叫做数据清理。数据清理指的是将数据从一种状态转变为另一种状态，且这些步骤是明确可逆的。它是为了将数据准备好以用于分析和可视化。

第三章，*数据探索*，解释了统计学是数据科学的核心，展示了 Julia 提供了多种统计功能。本章将对统计学做一个高级概述，并将解释如何使用 Julia 的统计包，如 Stats.jl 和 Distributions.jl，将这些统计概念应用于一般问题的技术。

第四章，*深入探讨推断统计学*，继续讲述统计学是数据科学的核心，并且 Julia 提供了多种统计功能。本章将对高级统计学做一个概述，然后解释如何使用 Julia 的统计包，如 Stats.jl 和 Distributions.jl，将这些统计概念应用于一般问题的技术。

第五章，*使用可视化理解数据*，解释了数据可视化是数据科学的重要组成部分，以及它如何使结果的沟通更加有效，并触及更广泛的受众。本章将介绍 Julia 中的 Vega、Asciiplot 和 Gadfly 包，它们用于数据可视化。

第六章，*有监督机器学习*，引述了汤姆·M·米切尔的名言：“如果一个计算机程序能够通过经验 E 来学习，并且在任务 T 中的表现（通过 P 衡量）随着经验 E 的增加而改进，那么我们就说它从经验中学习。”机器学习是一个研究领域，它赋予计算机学习和改进的能力，而无需明确编程。本章将解释 Julia 是一种高性能的高级语言，非常适合用于机器学习。本章将重点介绍有监督机器学习算法，如朴素贝叶斯、回归分析和决策树。

第七章，*无监督机器学习*，解释了无监督学习与有监督学习有所不同且更为复杂。其目的是让系统学习一些东西，但我们并不知道它会学到什么。本章将重点介绍无监督学习算法，如聚类。

第八章，*创建集成模型*，解释了一个团队比单个人更能做出更好的决策，尤其当每个团队成员都有自己的偏见时。机器学习也遵循这一规律。本章将重点讨论一种机器学习技术——集成学习，随机森林就是一个例子。

第九章，*时间序列*，展示了决策建模的能力，并解释了检查在一些实际应用中的关键作用，从重症监护室中的紧急医疗处理到军事指挥与控制系统。本章重点讨论时间序列数据和使用 Julia 进行预测。

第十章，*协同过滤与推荐系统*，解释了我们每天都面临决策和选择。这些选择可以从我们穿什么衣服到我们看什么电影，或者我们在网上点餐时吃什么。我们在商业中也做出决策。例如，我们应该投资哪只股票？如果决策能够被自动化，并且可以给我们提供合适的推荐呢？本章重点讨论推荐系统和诸如协同过滤和关联规则挖掘等技术。

第十一章，*深度学习简介*，解释了深度学习是一类通过利用多个非线性信息处理层进行无监督或有监督的特征提取、模式分析或分类的机器学习技术。本章将介绍如何在 Julia 中进行深度学习。深度学习是机器学习的一个新分支，其目标是——人工智能。我们还将了解 Julia 的深度学习框架 Mocha.jl，并学习如何利用它来实现深度学习。

# 本书所需的内容

读者需要一台拥有较新操作系统（推荐 64 位系统）、支持 Linux、Windows 7+或 Mac OS 的计算机，且需具备有效的互联网连接及安装 Julia、Git 和本书中使用的各种包的权限。

# 本书适合的读者

本书的标准读者群体是那些对 Julia 语言的基础知识了解较少的、希望探索如何利用 Julia 的生态系统进行数据科学的数据分析师和有志成为数据科学家的人员。此外，还有一些具备 Python 或 R 技能的用户，他们希望通过使用 Julia 提升进行数据科学的效率。我们期待读者具备一定的统计学和计算数学背景。

# 约定

本书中包含多种文本样式，用于区分不同类型的信息。以下是这些样式的示例及其解释。

文本中的代码词汇、数据库表名、文件夹名称、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 用户名均按以下方式显示：“Julia 还提供了一个名为`summarystats()`的函数。”

一段代码块设置如下：

```py
ci(x::HypothesisTests.FisherExactTest) 
ci(x::HypothesisTests.FisherExactTest, alpha::Float64)
ci(x::HypothesisTests.TTest) 
ci(x::HypothesisTests.TTest, alpha::Float64)
```

任何命令行输入或输出均按以下方式编写：

```py
julia> Pkg.update() 
julia> Pkg.add("StatsBase")

```

**新术语**和**重要词汇**以粗体显示。

### 注意

警告或重要说明会以如下框架形式出现。

### 提示

提示和技巧会以这样的方式展示。

# 读者反馈

我们始终欢迎读者的反馈。告诉我们您对本书的看法——您喜欢或不喜欢什么。读者反馈对我们来说非常重要，因为它帮助我们开发出能够让您真正从中受益的书籍。

若要向我们发送一般性反馈，只需发送电子邮件至 feedback@packtpub.com，并在邮件主题中注明书名。

如果您在某个领域拥有专长，并且有兴趣撰写或为书籍贡献内容，请查看我们的作者指南：[www.packtpub.com/authors](http://www.packtpub.com/authors)。

# 客户支持

现在，您已经成为 Packt 书籍的自豪拥有者，我们提供了多种方式帮助您充分利用您的购买。

## 下载示例代码

您可以从您的账户中下载本书的示例代码文件，网址是 [`www.packtpub.com`](http://www.packtpub.com)。如果您是在其他地方购买的本书，可以访问 [`www.packtpub.com/support`](http://www.packtpub.com/support)，注册后，我们会直接通过电子邮件将文件发送给您。

您可以按照以下步骤下载代码文件：

1.  使用您的电子邮件地址和密码登录或注册我们的网站。

1.  将鼠标指针悬停在顶部的 **SUPPORT** 标签上。

1.  点击 **代码下载与勘误**。

1.  在 **搜索** 框中输入书名。

1.  选择您想要下载代码文件的书籍。

1.  从下拉菜单中选择您购买本书的渠道。

1.  点击 **代码下载**。

下载文件后，请确保使用最新版本的工具解压或提取文件夹：

+   WinRAR / 7-Zip for Windows

+   Mac 用户请使用 Zipeg / iZip / UnRarX

+   Linux 用户请使用 7-Zip / PeaZip

本书的代码包也托管在 GitHub 上，地址为 [`github.com/PacktPublishing/Julia-for-data-science`](https://github.com/PacktPublishing/Julia-for-data-science)。我们还提供了其他书籍和视频的代码包，您可以在我们的丰富目录中找到，网址是 [`github.com/PacktPublishing/`](https://github.com/PacktPublishing/)。快去看看吧！

## 下载本书的彩色图片

我们还为您提供了一份 PDF 文件，其中包含本书中使用的截图/图表的彩色图片。这些彩色图片将帮助您更好地理解输出结果的变化。您可以通过 [`www.packtpub.com/sites/default/files/downloads/JuliaforDataScience_ColorImages.pdf`](http://www.packtpub.com/sites/default/files/downloads/JuliaforDataScience_ColorImages.pdf) 下载该文件。

## 勘误

尽管我们已经尽力确保内容的准确性，但错误还是会发生。如果您在我们的书籍中发现错误——可能是文本或代码中的错误——我们非常感谢您向我们报告。这样，您可以帮助其他读者避免困扰，并帮助我们改进后续版本。如果您发现任何勘误，请访问 [`www.packtpub.com/submit-errata`](http://www.packtpub.com/submit-errata) 提交，选择您的书籍，点击 **勘误提交表单** 链接，并输入您的勘误详情。一旦您的勘误被验证，您的提交将被接受，勘误将上传到我们的网站，或者添加到该书名的勘误部分中的现有勘误列表中。

要查看先前提交的勘误，请访问 [`www.packtpub.com/books/content/support`](https://www.packtpub.com/books/content/support)，并在搜索框中输入书名。所需的信息将在 **勘误** 部分下显示。

## 盗版

网络上侵犯版权的行为在所有媒体中都存在着持续性的问题。在 Packt，我们非常重视版权和许可证的保护。如果您在网上遇到任何我们作品的非法复制品，请立即向我们提供相关的地址或网站名称，以便我们采取措施。

请通过 copyright@packtpub.com 与我们联系，并提供涉嫌侵权材料的链接。

我们感谢您帮助保护我们的作者和我们提供有价值内容的能力。

## 问题

如果您对本书的任何部分有问题，可以通过 questions@packtpub.com 与我们联系，我们将尽力解决问题。
