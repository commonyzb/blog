---
title: "Markdown学习"
date: 2019-04-02T20:41:33+08:00
tags: ["markdown"]
categories: ["markdown"]
draft: false
---

# 1. 标题（Atx形式表示）

* 由n(1<=n<=6)个"# " 确定是n级标题。 

# 2. 字体样式

* 由字符 `*` 或字符 `_` 前后包裹的文字显示斜体文字。
* 由字符串`**` ,或字符串 `__` 前后包裹的文字显示粗体文字。
* 由字符串` ~~ ` 前后包裹的文字会被横线删除。

# 3. 段落和换行

* 一个markdown段落是由**一个或多个连续的文本行**组成，它的前后要有一个以上的空行。普通段落不该用空格或制表符来缩进。
* 缩进：可以用1个`TAB`键或者4个`space`键。
* 分隔符：可以用三个及以上的 `*`、 `-`、 `_`建立一个分割线。

4.列表
=============

4.1 无序列表
-------------

* "* " 、 "+ " 、 "- " 作为列表标记，可多级嵌套。
    例：
    * 无序列表
        * 无序列表
            * 无序列表


4.2 有序列表
-------------

* "n. " 设计各级列表及其嵌套（下级相对上级用4个空格或1个TAB键缩进)。
    例：
    1. Hello World
    2. Hello World
        1.Hello World
        2.Hello World
    3. Hello World
        3.1 Hello World

4.3 列表的一些小Tips：
---------------------

* 列表项目可包含多个段落，但每个项目下的段落必须缩进4个空格或者1个制表符。
* 如果要在列表项目内放进引用，那`>`就需要缩进。
* 如果要放代码区块的话，改区块就要缩进两次,即8个空格或是2个制表符。
* 一些特殊情况可以用转义字符`\`来化解。

# 5. 引用

* ` > ` 表示引用，引用可嵌套，在引用中可以使用其他的markdown语法
    例：正如苏轼所说:
    > 谁怕，一蓑烟雨任平生


6.代码块
==============

6.1 行内代码
--------------

* 行内代码：即使用 \`符号包裹代码。
* 例：
    `System.out.println("hello world");`

6.2 代码块：
-------------

* 代码块：即可以在代码块上面和下面添加 ` ``` `来表示代码块,或者简单缩进4个空格或是一个制表符即可。

* 语法高亮：在` ``` `后添加` 使用的语言 `即可。
    * 例：
    ```java 
    System.out.print("hello world");
    ```

* 代码行数：在` ``` `后添加 ` line-numbers `类就可以了。
    * 例：
    ```java {.line-numbers}
    System.out.println("hello world");
    ```

# 7.链接

* 链接内容定义的形式为：
    * 方括号（前面可以选择性地加上至多三个空格来缩进），里面输入链接文字。
    * 接着一个冒号。
    * 接着一个以上的空格或制表符。
    * 接着链接的网址。
    * 选择性地接着 title 内容，可以用单引号、双引号或是括弧包着。
    即``` [链接文字]: (网址 "描述信息") ```
    * 例：
    [Github]: https://github.com
    This is [my github homepage](https://github.com/commonyzb "github 主页") inline link.

# 8.图片

* 图片的表示形式：
    * 一个惊叹号`!`
    * 接着一个方括号，里面放上图片的替代文字
    * 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的`title`文字。
    * 即```![图片替代文字](图片地址 "描述信息")```

# 9.表格

* 语法：
```
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

# 10.参考

* [学习资料1]：https://www.appinn.com/markdown/#precode
* [学习资料2]：https://shd101wyy.github.io/markdown-preview-enhanced/#/zh-cn/markdown-basics