---
layout: post
title: 创造力的几个模型
date: 2018-7-20
cover_url: 
---

一篇对于之前博客[人工智能有创造力吗？](https://underwaternya.github.io/2017/11/09/is-this-creativity.html)的补充。来自书 *Switching Codes: Thinking Through Digital Technology in the Humanities and the Arts* 里面的 [“Logical Induction, Machine Learning, and Human Creativity”](https://books.google.co.uk/books?id=ZYPJXRW5nq0C&pg=PA140&dq=Logical+Induction,+Machine+Learning,+and+Human+Creativity&hl=en&sa=X&ved=0ahUKEwi3hc-lsq3cAhWK-mEKHbOGCmEQ6AEIKTAA#v=onepage&q=Logical%20Induction%2C%20Machine%20Learning%2C%20and%20Human%20Creativity&f=false) 。其中提到了创造力的四种模型。


### Exploratory
创造力就是从迷宫中找到出去的路。

Herbert Simon 认为所有创造力行为，都是基于一种解决问题的能力之上。他想象世界上存在一个巨大的 problem space（像是个巨大的迷宫），里面充满了人们未解的谜团。不管是人的智能，还是人工智能都是在试着从这个 problem space 走出去探索，指明一条路。

### Mathematica

许多数学家和逻辑学家，都认为创造力是一种重新解释问题的能力——换一种巧妙的视角，这个数学难题就能迎刃而解。比如如何快速分割正五边形？比如[残缺的棋盘](https://en.wikipedia.org/wiki/Mutilated_chessboard_problem)。换句话说，它会不会重新解读问题，换一种方法回答。


### Entropy-based（compression）
寻找一个出人意料的熵减方法。从大量事实中总结出一个最简单的道理。比如机器可以简单的总结出 97000 个 a 的规律。但是如果是 97000 个随机字符，结果就不一定那么简单。如果这 97000 个随机字符是从《麦克白》中抽取的，那么人类可以很简单的总结出来，机器就不可以。这其实就是[柯氏复杂性](https://zh.wikipedia.org/wiki/%E6%9F%AF%E6%B0%8F%E5%A4%8D%E6%9D%82%E6%80%A7)，它是衡量描述这个对象所需要的信息量的一个尺度。能快速减少复杂性的能力就是一种解决问题的能力，就是一种创造力。

### Compositional
组合，这就是我之前那篇文章[「人工智能可以有创造力吗？」](https://underwaternya.github.io/2017/11/09/is-this-creativity.html)中提到的。也称为 memory-based creativity。它需要两种能力：memory retrieval 和 case adaptation。前者是能从过去经验中取回记忆，后者是能巧妙地把两种东西连接起来，找到相同点（比如斯芬克斯，比如阿努比斯）。这种创造力和和 inductive reasoning 相关，都是从特殊到一般。这种切掉特殊走向一般的过程，意味着其中出现了信息损失。

这也是目前许多学者在研究的方向（比如机器学习生成美少女）。


