## 题目描述
Little Johnny was given a birthday present by his grandparents.

This present is a box of sticks of various lengths and colours.

Johnny wonders if there are three sticks in the set he has been given    that would form a triangle with different-coloured sides.

Let us note that Johnny is interested in non-degenerate triangles only, i.e.,    those with positive area.


## 输入格式
In the first line of the standard input an integer $k$ ($3\le k\le 50$) is given, which is the number of different colours of sticks.

The colours themselves are numbered from $1$ to $k$.

The following $k$ lines contain descriptions of the sticks of particular      colours.

The line no. $i+1$ holds integers that describe the sticks of colour $i$,separated by single spaces.

The first of these numbers, $n_i$ ($1\le n_i\le 1\ 000\ 000$), denotes the number of sticks of colour $i$.

It is followed, in the same line, by $n_i$ integers denoting the lengths of the sticks of colour $i$.All lengths are positive and do not exceed $1\ 000\ 000\ 000$.Furthermore, the total number of all sticks does not exceed $1\ 000\ 000$.


## 输出格式
Your program should print (on the first and only line of the standard output) either:

six integers, separated by single spaces, that describe the construction          of a triangle with different-coloured sides as follows:

the colour and the length of the first stick, the colour and the length          of the second stick, and the colour and the length of the third stick,                      or the word NIE (Polish for no) if no such triple of          sticks exists.

If there are multiple triples of different-coloured sticks that give rise      to a triangle, your program may pick one such triple arbitrarily.


## 题目大意
### 题目描述

小 Johnny 收到了祖父母送的生日礼物。

这个礼物是一盒各种长度和颜色的木棍。

Johnny 想知道，他收到的这些木棍中是否存在三根木棍，能够组成一个边长颜色各不相同的三角形。

需要注意的是，Johnny 只对非退化三角形感兴趣，即面积为正的三角形。

### 输入格式

输入的第一行包含一个整数 $k$（$3 \leq k \leq 50$），表示木棍的不同颜色数量。颜色本身编号为 $1$ 到 $k$。

接下来的 $k$ 行描述了每种颜色的木棍。第 $i+1$ 行描述了颜色为 $i$ 的木棍，包含若干个用空格分隔的整数。第一个整数 $n_i$（$1 \leq n_i \leq 1\,000\,000$）表示颜色为 $i$ 的木棍数量。随后是 $n_i$ 个整数，表示这些木棍的长度。所有长度均为正整数且不超过 $1\,000\,000\,000$。此外，所有木棍的总数不超过 $1\,000\,000$。

### 输出格式

你的程序应在标准输出的第一行（也是唯一一行）输出以下内容之一：

- 六个整数，用空格分隔，描述一个边长颜色各不相同的三角形的构造方式，依次为：第一根木棍的颜色和长度，第二根木棍的颜色和长度，以及第三根木棍的颜色和长度；  
- 或者输出单词 `NIE`（波兰语中的“无”），表示不存在这样的三根木棍。

如果存在多个满足条件的三根木棍，你的程序可以任意选择其中一个输出。

```input1
4
1 42
2 6 9
3 8 4 8
1 12
```

```output1
3 8 4 12 2 9
```

