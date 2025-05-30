# 题目描述

CSP 即将开始了，小云打算开始好好读书！~~现在开始读书是不是有点晚了~~

别急！小云兴高采烈地翻开了一部英文名著：`C++ Primer Plus`！她准备认真研读。但当她打开书后发现，书中的字符串都乱套了。有的地方大小写错了，有的地方空格多了，有的地方冒出来了很多换行。

有强迫症的小云决定开始修复这部名著！

具体的，小云会选择接下来书上的一个段落 $s$。段落 $s$ 是一个由多行、多个单词组成的字符串。单词与单词之间由一个或多个**空格**与**换行**分隔。单词的定义包括以下两类字符串：

- 英文单词。仅包含英文字符的字符串。例如 `AbCdEfG`。
- 标点符号。仅包含单个标点符号的字符串。例如 `,`。

对于给定的段落 $s$ ，你需要完成以下任务：

- （1）修正字符串中的**每个英文单词**。使**每个英文单词均变为首字母大写，其余字母小写**。
- （2）移除字符串中所有的**多余空格**（即每两个单词之间**只保留一个空格，首尾没有多余空格**）。
- （3）移除字符串内所有的**换行**和**空行**。
- （4）将全部标点符号**与其前一个英文单词紧贴**，并**在该标点符号之后留下一个空格**。保证转换后的结果不存在连续多个标点符号的情况。
- （5） 其余字符均不做任何改动，但位置可能会随着空格的删除而前移。

现在，小云想知道处理后的字符串是什么。你能帮帮小云吗？保证整个段落的第一个单词一定为英文单词。

# 输入格式

输入共若干行，用于表示一个字符串 $s$。含义见【题目描述】。

# 输出格式

共 $1$ 行一个字符串，表示修复处理后的字符串。

# 样例 1
## 输入
```
hello   world  !    this is   C   !
```
## 输出
```
Hello World! This Is C!
```

# 样例 2
## 输入
```
hello   world  !

   this  is

a     te

st .  
```
## 输出
```
Hello World! This Is A Te St.
```

# 样例 3

## 输入

[ex_b.in](./5390/file/ex_b.in)

[ex_b.out](./5390/file/ex_b.out)

# 数据范围

对于 $100\%$ 的数据，字符串 $s$ 长度 $\le 500$，给出的字符串行数不会超过 $50$，串中字符包含 `a~z`，`A~Z`，`+`，`-`，`,`，`.`，`!`，`?`，`'` 以及空格和换行。
