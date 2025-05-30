## 题目描述


Curiosity is the rover that explores the Gale Crater on Mars. Recently it found an evidence of water in Martian soil, which will make it easier to plan the future manned missions. $ $

Curiosity can communicate with Earth directly at speeds up to $32 Kbit/s$ , but on average $14$ minutes and $6$ seconds will be required for signals to travel between Earth and Mars.

`You have just seen a stone and applied brakes, but you know that the rover is already passing that stone` -- Matt Heverly, the rover's driver, explains. `So we just plan the route, then write down a list of simple textual commands: move one meter ahead, turn left, make a photo and so on`.

Sometimes it is necessary to react very fast to some unexpected events. For example, if the cameras have seen something interesting, then you might want to change the route of the rover to make an additional photo. To do that, you send a substitution command of the form $s/〈string〉/〈replacement〉/g$ . This replaces all occurrences of $〈string〉,$ starting with the leftmost one, to $〈replacement〉.$

More formally, if A is a non-empty string and $B$ is a string, then to apply the substitution command $s/A/B/g$ to a string $S$ , you should do the following:

Find the leftmost occurrence of A in $S$ , such that $S =$ SL $+$ A $+$ SR.

If there is no such occurrence, stop. Then, $S$ is the answer.

Let $R$ be the result of applying $s/A/B/g$ to SR.

The answer is SL $+ B + R$ .

This means that:

If there are two overlapping occurrences of A in $S$ , only the leftmost one is replaced. For example, applying $`s/aba/c/g`$ to `abababa` yields `cbc`: after replacing the first occurrence of `aba` the string turns to `cbaba`, and only the last occurrence of `aba` can be replaced after that.

No substitution uses the results of previous substitutions. For example, applying $`s/a/ab/g`$ to `a` yields `ab`, applying $`s/a/ba/g`$ to `a` yields `ba`.

You know that the longer is the command, the bigger is the time necessary to transmit it. So, you have to write a program that finds shortest command that transforms the initial string to the final string.



## 输入格式


The first line contains the initial and the final strings. Both strings are non-empty and their lengths do not exceed $2000$ characters. The strings contain only English letters, spaces and punctuation signs (commas, colons, semicolons and hyphens: $‘,', ‘:', ‘;', ‘-').$ The given strings are not equal.



## 输出格式


Output the substitution command that transforms initial string to final string and has the minimum length. If there are several shortest substitution commands, output any of them.



## 题目大意
# [NWRRC2013] Correcting Curiosity

## 题目描述

“好奇号”是探索火星上盖尔陨石坑的火星车。最近，它在火星土壤中发现了水存在的证据，这将使未来的火星登陆任务变得更加容易。$ $

“好奇号”可以用高达$32 Kbit/s$的速度与地球直接通信 ，但在地球和火星之间传输信号分别平均需要$14$秒和$6$秒。

`你刚刚看到一块石头并踩下了刹车，但你知道火星车已经经过那块石头了` -- 火星车司机Matt Heverly解释道。`所以我们需要规划路线，然后写下一个简单的命令列表：如向前移动一米，左转，拍照等等`.

有时你有必要对一些突发事件做出非常迅速的反应。例如，当相机看到了一些有趣的东西，那么你可能会想改变火星车的路线来拍摄的照片。为此，您需要发送一个形式为 $s/〈string〉/〈replacement〉/g$ . 这将替换所有出现的 $〈string〉,$ 从最左边的开始, 到 $〈replacement〉.$

更确切地说，如果A是非空字符串，而$B$是字符串, 则要将替换命令$s/A/B/g$应用于字符串$s$，执行以下操作：

在$S$中查找最左边出现的A，这样$S=$SL$+$A$+$SR。

如果没有A，请停止操作。$S$就是答案。

让$R$成为对SR应用$s/A/B/g$的结果。

那么答案是SL$+B+R$。

这就说明:

如果在$S$中有两个重叠的A，那么只替换最左边的一个。例如，将$`s/aba/c/g`$应用于`abababa`会产生`cbc`：在替换第一个`aba `之后，字符串将变为`cbaba `，在此之后只能替换最后一个出现的` aba `。

如果没有替换就使用先前替换的结果。例如，将$`s/a/ab/g`$应用于`a`产生`ab`，将$`s/s/a/ba/g`$应用于`a`产生`ba`。

命令越长，传输它所需的时间就越长。因此，需要你编写一个程序，找到最短的命令，将初始字符串转换为最终字符串。

## 输入格式

第一行输入包含初始字符串和最终字符串。这两个字符串都不是空的，并且它们的长度不超过$2000$。字符串仅包含英文字母、空格和标点符号（逗号、冒号、分号和连字符：$'，'，'：'，'；'，'-'）。$给定的字符串不相同。

## 输出格式

输出将初始字符串转换为最终字符串并最短的替换命令。如果有多个最短的替换命令，请输出其中任何一个。

## 样例 #1

### 样例输入 #1

```
move left, move right; move up
move left, move down, move up
```

### 样例输出 #1

```
s/right;/down,/g
```

## 样例 #2

### 样例输入 #2

```
If not found: move x; else move -x
If found: move x; else move -x
```

### 样例输出 #2

```
s/ not//g
```

## 样例 #3

### 样例输入 #3

```
abababa
cbc
```

### 样例输出 #3

```
s/aba/c/g
```

## 提示

时间限制: 2 s, 内存限制: 256 MB.

```input1
move left, move right; move up
move left, move down, move up

```

```output1
s/right;/down,/g

```

```input2
If not found: move x; else move -x
If found: move x; else move -x

```

```output2
s/ not//g

```

```input3
abababa
cbc

```

```output3
s/aba/c/g

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



