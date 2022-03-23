---
title: "内嵌 Orbit 测试"
date: 2022-03-19T00:00:00+08:00
description: "一个简单的内嵌卡片测试"
tags: ["test"]
---

简单测试一下Orbit能不能在GitHubPage上显示。

<!--more-->

Orbit是Andy的实验性助记媒介平台。本页面用于测试Orbit能否在GitHubPages上使用。

{{< withorbit >}}
    <orbit-prompt
            question="Andy的实验性助记媒介平台叫什么？"
            answer="Orbit"
    ></orbit-prompt>
    <orbit-prompt
            question="这个页面是做什么用的？"
            answer="测试Orbit能不能在GithubPages上使用"
    ></orbit-prompt>
{{< /withorbit >}}

如果你看到上面的 Orbit 页面，本测试就成功了～
