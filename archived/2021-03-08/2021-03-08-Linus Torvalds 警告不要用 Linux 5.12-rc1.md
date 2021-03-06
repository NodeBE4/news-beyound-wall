---
layout: post
title: "Linus Torvalds 警告不要用 Linux 5.12-rc1"
date: 2021-03-08T02:32:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=67131
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1615170720000-->
[Linus Torvalds 警告不要用 Linux 5.12-rc1](https://www.solidot.org/story?sid=67131)
------

<div>
Linus Torvalds 在邮件列表上<a href="https://lwn.net/ml/linux-kernel/CAHk-=wjnzdLSP3oDxhf9eMTYo7GF-QjaNLBUH1Zk3c4A7X75YA@mail.gmail.com/" target="_blank">紧急呼吁</a>用户<a href="https://arstechnica.com/gadgets/2021/03/psa-linux-folks-stay-away-from-the-5-12-rc1-kernel/" target="_blank">不要使用</a>最近释出的 Linux 5.12-rc1。他表示，在公开的 git 树上，v5.12-rc1 的标签被重命名为 v5.12-rc1-dontuse， dontuse 意味着不要使用，因为该版本破坏了交换文件 swapfile 的处理，会导致文件系统无法使用。当内核将内存中的内容交换写入到磁盘上，数据会随机写入 swapfile 所在的相同磁盘和分区，它不仅会覆写现有文件的数据，而且还会覆写破坏元数据，可能导致整个文件系统无法挂载和使用。Torvalds 称，如果你不使用交换文件，或者使用的是交换分区而不是交换文件，那么你不会受到影响。<p><img src="https://img.solidot.org//0/446/liiLIZF8Uh6yM.jpg" height="120" style="display:block"/></p>
</div>
