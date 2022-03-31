本文将在知乎同步更新，但在本网站上将搭配助记媒介进行

# 认识数学软件

许多人对进行解决数学问题的初映像，还停留在一个这么一个映像：一个人待在一个房间里，满屋子除了草稿纸不见他物，做题的人拿着纸币在草稿纸上疯狂的计算。实际上这跟我们的数学教育可能有一定的关系，由于需要参加考试，为了保证公平性，往往只允许使用一些比较初等的计算器，因此不少人将计算机和数学一分为二了。但实际上，随着科技的发展，许多的工作都可以由计算机完成，特别是面对数字量大，复杂度高的问题是，计算机更显得游刃有余。许多认为计算机无法完成的事情，计算机都可以帮你完成，例如求导，积分，解方程组。

本文将着重介绍一下最常用的三个工具：matlab,mathematica,python

## matlab的历史

了解matlab的历史，是有助于帮我们理解matlab的这款软件本身的优点和缺点

实际上这段历史在matlab的官网上有创始人的个人陈述，在这里我讲截取一部分

[MATLAB发展简史 - MATLAB & Simulink (mathworks.cn)](https://ww2.mathworks.cn/company/newsletters/articles/a-brief-history-of-matlab.html)

根据matlab创始人Cleve Moler本人所言

> 在70年代和80年代初期，我在新墨西哥大学教授线性代数和数值分析。我希望我的学生能够方便地使用LINPACK和EISPACK，而不必编写Fortran程序。我所说的“方便地使用”是指无需执行远程批处理和重复的编辑-编译-链接-加载-执行过程，而校园中央主机计算机一般需要执行这个过程。
>
> 因此，我研读了Niklaus Wirth的著作《*Algorithms + Data Structures = Programs*》，学习如何解析编程语言。我用Fortran编写了初版MATLAB——矩阵实验室（Matrix Laboratory）的缩写，其数据类型只有矩阵。这个项目对我来说是兴趣爱好，也是我希望了解的编程新领域，并且可以给我的学生学习使用。那时候我没有任何正式的外部支持，当然也没有商业计划。
>
> 初版MATLAB只是一个交互式矩阵计算器。下面这个启动屏幕展示了所有保留的文字和函数，只有71个。要添加其他函数，用户必须从我这里获取源代码、编写Fortran子程序、在解析表里添加自己的函数名称，然后重新编译MATLAB。

q:初版的matlab是干什么用的

a:交互式矩阵计算器

q:初版的matlab的全程

a:matrix laboratory

在这里我要强调一下matlab的初版的用途：矩阵计算，在以后matlab的学习过程中，你会发现，矩阵计算一直是无法绕开的问题，因为matlab的基石便是矩阵计算。我们也可以看到初版matlab的成功正式因为其优秀的矩阵运算能力

> 1979-80学年我在斯坦福任教，在那里教授数值分析的研究生课程，并在课程中引入了这一矩阵计算器。一些学生也在学习控制理论和信号处理等课程，而我对这些内容一无所知。但是，这些课程涉及的数学以矩阵运算为核心，因此MATLAB迅速得到了学生的追捧。

这么优秀的软件最终在众人的帮助下开始商业化

> 终于，PC-MATLAB于1984年在拉斯维加斯举行的IEEE决策与控制会议（IEEE Conference on Decision and Control）上首次发布。次年，发布了针对Unix工作站的Pro-MATLAB。



## mathematica历史

mathematica在网络上就比较难找了（特别是中文互联网），许多内容我并没有找到原文的出处，为了严谨起见，我就并没有作为参考

我们直接来看mathemtica官方的版本更新说明，我会摘取重要的几条

[Mathematica 最新版本和旧版本历史 (wolfram.com)](https://www.wolfram.com/mathematica/quick-revision-history.html)

> 1988年6月，Mathematica 首版发布
>
> 1989年8月：支持远程内核
>
> 1991年1月，增加功能：笔记本前端，数值常微分方程求解器，增加 ParametricPlot3D
>
> 1992年6月
>
> - Unix 平台的 WSTP（Wolfram Symbolic Transfer Protocol）增强功能和文档
> - Macintosh 平台的 WSTP（Wolfram Symbolic Transfer Protocol）
>
> 1993年6月：具有新笔记本命令的 Windows 前端
>
> 1996年9月：交互式数学排版系统

q:初版mathematica发布时间

a:1988年(80年代末)

q:mathematica更新较多的内容是

a：笔记本

q:1989年8月发布的新功能（第一次更新中增加的功能）

a:远程内核

我们可以发现,mathematica讲所有的更新方向，都集中于交互，图像，笔记本上

所以说通常在使用上，mathematica会比较的容易，而且mathematica的帮助文档的质量也是数一数二的，搭配上wolfram自家的mathworld，你甚至可以不看教材就可以学会数学

同时我们也可以看到，mathematica首次更新就增加了远程内核功能，也说明开发者本身，在开发的过程中，就并没有打算让用户在自己的电脑上完成所有的程序运算，这一点与matlab截然不同，因此我们也可以看到，mathematica在对速度和内存的优化上，并没有下多大功夫

## python

python实际上不是数学软件，他是一种编程语言，但是在拥有numpy,pandas等一系列的库后，python就拥有了和matlab，mathematica这些商业软件掰掰手腕的能力

根据知乎用户 xue gy的回答  [MATLAB在逐渐被Python淘汰吗？](https://www.zhihu.com/question/367881424/answer/2415598493)

在大部分的场景下，python基本上都是会比matlab快的，特别在解微分方程上。

## 那为什么我们使用matlab

但这并不代表说matlab就一无用处，会被淘汰

q:PC-matlab的发行时间

a:上世纪80年年代(1984)

正因为发行时间早，使用用户多，相应的在稳定性上matlab是有保证的，评论区中也提到python在画图的过程中有时会出问题，而且数据量大的时候会出现故障。

q:matlab比python好在哪里

a:稳定性上

matlab上的simulink现在更是matlab的最核心的功能，在控制系统建模、仿真上广泛的应用，这种应用是通常是无法替代的。试想一下，飞机上的控制功能软件，是使用虽然慢但是稳定的matlab好呢，还是使用快但是可能出问题的python呢？

而且python上的帮助文档是不如matlab来的有序的，这也给上手的人带来了巨大的麻烦

## 关于mathematica

实际上我本人是很喜欢mathematica，语言的简洁易用，特别详尽的帮助文档（甚至可以说是教科书级别），上手难度非常低（mathematica的函数非常多，基本上涵盖了数学的方方面面），而且mathematica在符号计算上的能力是非常强的，可以直接把未知数放进方程中直接进行计算，像学生比较头疼的不定积分，微分方程解析解，都可以直接算出来，不过遗憾的是，他的应用的场景还比较少，同时计算的也比较慢一些，所以说本人通常将mathematica当草稿纸使用，在一些不太确定的情况下利用mathematica进行验算。后期我也会写关于mathematica的教程

q:mathematica什么计算上的能力很强

a:符号计算

## 为什么我要写matlab教程

因为考试要考(逃)

