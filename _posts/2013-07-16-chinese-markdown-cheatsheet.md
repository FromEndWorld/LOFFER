---
layout: post
title: Markdown语法简介
date: 2013-07-16
Author: Shengbin 
tags: [sample, markdown]
comments: true
toc: true
---

本中文版Markdown语法简介来自博客 <https://blog.shengbin.me/posts/markdown-syntax>

Markdown语法的完整介绍在这里：<http://daringfireball.net/projects/markdown/syntax>。下面整理的这些为了方便写博客时参考。

## 分段与分行

以一个或多个空行来隔开段落；以两个或多个空格来段内换行。

## 标题

```
This is an H1
=============

This is an H2
-------------

# This is an H1

##  This is an H2

######  This is an H6

```

## 引用

在每一行前面写一个`>`：

```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

```

效果：

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

或者在每一段前面写一个`>`：

```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

```

## 多重引用

```
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

```

效果：

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

## 列表

列表项占一行，以*、+、-开头即可：

```
*   Red
*   Green
*   Blue

```

效果：

-   Red
-   Green
-   Blue

有序列表只需要将上述标记符换成数字加句点。而且顺序由书写顺序决定，与数字无关，但数字需要从1开始。例如：

```
1\.  Bird
3.  McHale
2.  Parish

```

效果：

1.  Bird
2.  McHale
3.  Parish

每一个列表项可以多行：

```
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.

```

效果：

-   Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
-   Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

## 代码块

每一行前面缩进四个或以上个空格，就认为是开始了一段代码块。代码块内原样输出。

```
This is a normal paragraph:

    This is a code block.

```

效果：

This is a normal paragraph:

```
This is a code block.

```

## 横线

三个或更多个`*`、`-`（它们之间可以有空格）会产生横线：

```
* * *

```

效果：

* * * * *

## 链接

内嵌链接：

```
I get 10 times more traffic from [Google](http://google.com/ "Google")
than from [Yahoo](http://search.yahoo.com/ "Yahoo Search") or
[MSN](http://search.msn.com/ "MSN Search").

```

或参考文献式链接（缺省的链接标记认为与文本一致）：

```
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"

I get 10 times more traffic from [Google][] than from
[Yahoo][] or [MSN][].

  [google]: http://google.com/        "Google"
  [yahoo]:  http://search.yahoo.com/  "Yahoo Search"
  [msn]:    http://search.msn.com/    "MSN Search"

```

效果：

I get 10 times more traffic from [Google](http://google.com/ "Google") than from [Yahoo](http://search.yahoo.com/ "Yahoo Search") or [MSN](http://search.msn.com/ "MSN Search").

如果直接以链接地址作为链接文本，可以用如下快捷写法：

```
<http://www.shengbin.me> 效果：

```

[http://www.shengbin.me](http://www.shengbin.me/)

## 强调

单个`*`或`_`产生斜体，两个（`**`、`__`）则产生粗体。例如：

```
*like* _this_

**like** **this**

```

效果：

*like* *this*

**like** **this**

## 内嵌代码

```
code: `echo hello`

```

效果：

code: `echo hello`

## 图片

图片与链接类似，只需在文本前面加上感叹号`!`即可。图片位置和大小无法通过Markdown来指定。

## 转义字符

以下特殊字符需要用`\`转义得到。

```
\   backslash
`   backtick
*   asterisk
_   underscore
{}  curly braces
[]  square brackets
()  parentheses
#   hash mark
+   plus sign
-   minus sign (hyphen)
.   dot
!   exclamation mark
```