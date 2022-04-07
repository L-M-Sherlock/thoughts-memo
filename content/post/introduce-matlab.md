---
title: "认识 MATLAB"
date: 2022-03-31T11:53:12+08:00
description: ""
tags: ["数学"]
---

本文将在知乎同步更新，但在本网站上将搭配助记媒介进行

# 认识数学软件

许多人对进行解决数学问题的初映像，还停留在一个这么一个映像：一个人待在一个房间里，满屋子除了草稿纸不见他物，做题的人拿着纸币在草稿纸上疯狂的计算。实际上这跟我们的数学教育可能有一定的关系，由于需要参加考试，为了保证公平性，往往只允许使用一些比较初等的计算器，因此不少人将计算机和数学一分为二了。但实际上，随着科技的发展，许多的工作都可以由计算机完成，特别是面对数字量大，复杂度高的问题是，计算机更显得游刃有余。许多认为计算机无法完成的事情，计算机都可以帮你完成，例如求导，积分，解方程组。

本文将着重介绍一下最常用的三个工具：MATLAB, mathematica, python

## MATLAB 的历史

了解 MATLAB 的历史，是有助于帮我们理解 MATLAB 的这款软件本身的优点和缺点

实际上这段历史在 MATLAB 的官网上有创始人的个人陈述，在这里我讲截取一部分

[MATLAB发展简史 - MATLAB & Simulink (mathworks.cn)](https://ww2.mathworks.cn/company/newsletters/articles/a-brief-history-of-MATLAB.html)

根据 MATLAB 创始人 Cleve Moler 本人所言

> 在 70 年代和 80 年代初期，我在新墨西哥大学教授线性代数和数值分析。我希望我的学生能够方便地使用 LINPACK（数值线性代数的库，计算方程组，矩阵分解，矩阵乘法）和 EISPACK（计算特征值的 Fortran 库），而不必编写 Fortran 程序。我所说的“方便地使用”是指无需执行远程批处理和重复的编辑-编译-链接-加载-执行过程，而校园中央主机计算机一般需要执行这个过程。
>
> 因此，我研读了 Niklaus Wirth 的著作《*Algorithms + Data Structures = Programs*》，学习如何解析编程语言。我用 Fortran 编写了初版 MATLAB——矩阵实验室（Matrix Laboratory）的缩写，其数据类型只有矩阵。这个项目对我来说是兴趣爱好，也是我希望了解的编程新领域，并且可以给我的学生学习使用。那时候我没有任何正式的外部支持，当然也没有商业计划。
>
> 初版 MATLAB 只是一个交互式矩阵计算器。下面这个启动屏幕展示了所有保留的文字和函数，只有 71 个。要添加其他函数，用户必须从我这里获取源代码、编写 Fortran 子程序、在解析表里添加自己的函数名称，然后重新编译 MATLAB。


{{< withorbit >}}
    <orbit-prompt
            question="初版的 MATLAB 主要解决什么数学问题"
            answer="矩阵的计算"
    ></orbit-prompt>
     <orbit-prompt
            question="编写 MATLAB 的初衷是辅助学生使用什么程序"
            answer="线性代数相关的 Fortran 库(回答 LINPACK, EISPACK 也可)"
    ></orbit-prompt>
    <orbit-prompt
            question="MATLAB 辅助学生使用一些线性函数相关的 Fortran 库，其「辅助」指的是什么"
            answer="省去远程批处理和编译等工作"
    ></orbit-prompt>
    <orbit-prompt
            question="MATLAB 的全称是什么？"
            answer="matrix laboratory"
    ></orbit-prompt>
     <orbit-prompt
            question="初版 MATLAB 的可拓展性不好，需要用户获取源代码，编写子程序，并重新编译 MATLAB"
            answer=""
    ></orbit-prompt>
{{< /withorbit >}}

在这里我要强调一下 MATLAB 的初版的用途：矩阵计算，在以后 MATLAB 的学习过程中，你会发现，矩阵计算一直是无法绕开的问题，因为 MATLAB 的基石便是矩阵计算。我们也可以看到初版 MATLAB 的成功正式因为其优秀的矩阵运算能力

> 1979-80学年我在斯坦福任教，在那里教授数值分析的研究生课程，并在课程中引入了这一矩阵计算器。一些学生也在学习控制理论和信号处理等课程，而我对这些内容一无所知。但是，这些课程涉及的数学以矩阵运算为核心，因此 MATLAB 迅速得到了学生的追捧。

这么优秀的软件最终在众人的帮助下开始商业化

> 终于， PC-MATLAB 于1984年在拉斯维加斯举行的 IEEE 决策与控制会议（IEEE Conference on Decision and Control）上首次发布。次年，发布了针对 Unix 工作站的 Pro-MATLAB 。



## mathematica历史

mathematica在网络上就比较难找了（特别是中文互联网），许多内容我并没有找到原文的出处，为了严谨起见，我就并没有作为参考

我们直接来看 mathemtica 官方的版本更新说明，我会摘取重要的几条

[Mathematica 最新版本和旧版本历史 (wolfram.com)](https://www.wolfram.com/mathematica/quick-revision-history.html)

> 1988年 6 月，Mathematica 首版发布
>
> 1989年 8 月：支持远程内核
>
> 1991年 1 月，增加功能：笔记本前端，数值常微分方程求解器，增加 ParametricPlot3D
>
> 1992年 6 月
>
> - Unix 平台的 WSTP（Wolfram Symbolic Transfer Protocol）增强功能和文档
> - Macintosh 平台的 WSTP（Wolfram Symbolic Transfer Protocol）
>
> 1993年 6 月：具有新笔记本命令的 Windows 前端
>
> 1996年 9 月：交互式数学排版系统

{{< withorbit >}}
    <orbit-prompt
            question="初版 mathematica 发布时间"
            answer="1988年(80年代末)"
    ></orbit-prompt>
    <orbit-prompt
            question="mathematica 更新较多的内容是"
            answer="笔记本"
    ></orbit-prompt>
    <orbit-prompt
            question="1989 年 8 月发布的新功能（第一次更新中增加的功能）"
            answer="远程内核"
    ></orbit-prompt>
{{< /withorbit >}}

我们可以发现, mathematica 讲所有的更新方向，都集中于交互，图像，笔记本上

所以说通常在使用上， mathematica 会比较的容易，而且 mathematica 的帮助文档的质量也是数一数二的，搭配上 wolfram 自家的 mathworld, 你甚至可以不看教材就可以学会数学

同时我们也可以看到， mathematica 首次更新就增加了远程内核功能，也说明开发者本身，在开发的过程中，就并没有打算让用户在自己的电脑上完成所有的程序运算，这一点与 MATLAB 截然不同，因此我们也可以看到， mathematica 在对速度和内存的优化上，并没有下多大功夫

## python

python 实际上不是数学软件，他是一种编程语言，但是在拥有 numpy, pandas 等一系列的库后， python 就拥有了和 MATLAB, mathematica 这些商业软件掰掰手腕的能力 

根据知乎用户 xue gy的回答  [MATLAB 在逐渐被 Python 淘汰吗？](https://www.zhihu.com/question/367881424/answer/2415598493)

在大部分的场景下， python 基本上都是会比 MATLAB 快的，特别在解微分方程上。

## 那为什么我们使用MATLAB

但这并不代表说 MATLAB 就一无用处，会被淘汰


{{< withorbit >}}
    <orbit-prompt
            question="PC-MATLAB 的发行时间"
            answer="上世纪 80 年年代(1984)"
    ></orbit-prompt>
{{< /withorbit >}}

正因为发行时间早，使用用户多，相应的在稳定性上 MATLAB 是有保证的，评论区中也提到 python 在画图的过程中有时会出问题，而且数据量大的时候会出现故障。

{{< withorbit >}}
    <orbit-prompt
            question="MATLAB 比 python 好在哪里"
            answer="稳定性上"
    ></orbit-prompt>
{{< /withorbit >}}

MATLAB上的 simulink 现在更是 MATLAB 的最核心的功能，在控制系统建模、仿真上广泛的应用，这种应用是通常是无法替代的。试想一下，飞机上的控制功能软件，是使用虽然慢但是稳定的 MATLAB 好呢，还是使用快但是可能出问题的 python 呢？

而且 python 上的帮助文档是不如 MATLAB 来的有序的，这也给上手的人带来了巨大的麻烦

## 关于mathematica

实际上我本人是很喜欢 mathematica ，语言的简洁易用，特别详尽的帮助文档（甚至可以说是教科书级别），上手难度非常低（ mathematica 的函数非常多，基本上涵盖了数学的方方面面），而且 mathematica 在符号计算上的能力是非常强的，可以直接把未知数放进方程中直接进行计算，像学生比较头疼的不定积分，微分方程解析解，都可以直接算出来，不过遗憾的是，他的应用的场景还比较少，同时计算的也比较慢一些，所以说本人通常将 mathematica 当草稿纸使用，在一些不太确定的情况下利用 mathematica 进行验算。后期我也会写关于 mathematica 的教程

{{< withorbit >}}
    <orbit-prompt
            question="mathematica什么计算上的能力很强"
            answer="符号计算"
    ></orbit-prompt>
{{< /withorbit >}}

## 为什么我要写 MATLAB 教程

因为考试要考(逃)

