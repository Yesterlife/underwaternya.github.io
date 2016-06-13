---
layout: post
title: Cover 子主题制作记录
date: 2016-6-13 15:11:00
---

之前一直谋划着给现在用的 Cover 做一个 child theme，最近终于空下来开始做。这里记录一下制作过程和还是不甚明确的点。

使用了 Child Theme Configurator 这个插件，它能创造、设置子主题。就用它直接生成了 cover-child。（本来直接在 wp-content/themes 里添加了 cover-child 文件夹，但是 Wordpress 后台却没有显示。后来经提醒才发现是要手动在网页后台上传一个压缩包才行。）

你也能在这个子主题制造插件里选择复制原主题的一些 PHP 文件，比如 footer.php 之类的，以免更新原主题时这些设置也被更新。需要注意的是它不能复制所有的 PHP 文件。

> Copy PHP templates from the parent theme by selecting them here. The Configurator defines a template as a Theme PHP file having no PHP functions or classes. Other PHP files cannot be safely overridden by a child theme.

似乎是其中带有 PHP functions 和 classes 的文件不能复制。这就比较麻烦了。我们自定义了 header.php，而它似乎是带有了函数。根据上面的描述，子主题的 header.php 不能安全覆盖原主题。这是没有解决的问题之一，现在也是在更新 Cover 之后，手动在 FTP 替换了 header.php。

第二个手动替换的内容是 style.css。因为在早期修改样式的时候，我们都直接修改了原主题的 style.css；修改的内容实在太多，导致挑不出哪些是后来修改的，哪些是原来的。于是我暴力地把两个主题的 CSS 文件都替换成了原来的……

第三个是 template-tags.php，我把原来的 Previous Post 改成了「下一篇」，Next Post 直接删了。这个也是一个未解之谜，不知为何没有覆盖成功。

随之而来的问题还有在 Aesop 这个主题绑定的插件中，有些原来的样式不见/失效了。之后又加了几行样式。

诶，记一次能力范围外的升级……不过 PHP 没有动力搞懂啊。 

