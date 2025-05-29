## 题目描述
Byteasar once decided to start manufacturing necklaces.

He subsequently bought a very long string of colourful coral beads for a bargain price.

Byteasar now also has a machine that, for a given ![](http://main.edu.pl/images/OI17/kor-en-tex.1.png) (![](http://main.edu.pl/images/OI17/kor-en-tex.2.png)), can cut the string    into pieces (or substrings) of ![](http://main.edu.pl/images/OI17/kor-en-tex.3.png) coral beads (i.e., the first piece consists of the beads no.

![](http://main.edu.pl/images/OI17/kor-en-tex.4.png), the second of ![](http://main.edu.pl/images/OI17/kor-en-tex.5.png), etc.).

If the length of the string (measured in coral beads) is not a multiple of ![](http://main.edu.pl/images/OI17/kor-en-tex.6.png),    then the last piece is not used, as it has length smaller than ![](http://main.edu.pl/images/OI17/kor-en-tex.7.png).

From now on we denote the colours of the beads with positive integers.

Byteasar, always praising diversity, wonders how he should choose the number ![](http://main.edu.pl/images/OI17/kor-en-tex.8.png)    in order to get as many different substrings as possible.

The ends of the long string that will be cut are different: there are specific    beginning and ending (rather than two interchangeable endpoints), and the machine    of course starts cutting at the beginning. On the other hand, in the substrings    obtained from cutting the endpoints are interchangeable, and so the substrings    can be reversed. In other words, the substrings ![](http://main.edu.pl/images/OI17/kor-en-tex.9.png) and ![](http://main.edu.pl/images/OI17/kor-en-tex.10.png) are    identical to us. Write a program that determines the optimum value of ![](http://main.edu.pl/images/OI17/kor-en-tex.11.png) for Byteasar.

## 输入格式
In the first line of the standard input there is an integer ![](http://main.edu.pl/images/OI17/kor-en-tex.37.png)      (![](http://main.edu.pl/images/OI17/kor-en-tex.38.png)) denoting the length of the string to cut.

In the second line there are ![](http://main.edu.pl/images/OI17/kor-en-tex.39.png) positive integers ![](http://main.edu.pl/images/OI17/kor-en-tex.40.png)      (![](http://main.edu.pl/images/OI17/kor-en-tex.41.png)), separated by single spaces, that denote      the colours of successive beads in Byteasar's string.


## 输出格式
Two integers, separated by a single space, should be printed out to the first line of the standard ouput:

the (maximum) number of different substrings that can be obtained with an optimal choice    of parameter ![](http://main.edu.pl/images/OI17/kor-en-tex.42.png), and the number ![](http://main.edu.pl/images/OI17/kor-en-tex.43.png) of such optimal values of ![](http://main.edu.pl/images/OI17/kor-en-tex.44.png).

The second line should contain ![](http://main.edu.pl/images/OI17/kor-en-tex.45.png) integers separated by single spaces:

the values of parameter ![](http://main.edu.pl/images/OI17/kor-en-tex.46.png) that yield an optimum solution;    these can be given in arbitrary order.

输出两行，第一行第一个数为最多可以得到的不同子串的个数，第二个数为取到最优解时的不同的k的个数。第二行包含若干个数，为取到最优解时的不同的k 。第二行中的不同的k可以按任意位置输出。


## 题目大意
### 【题目描述】

Byteasar 有 $n$ 个珠子，第 $i$ 个颜色为 $a_i$，和一台机器。

Byteasar 可以选定一个值 $k$，然后机器会让 $1\sim k$ 的珠子组成项链 $b_1$，$k+1\sim 2k$ 的珠子组成项链 $b_2$，以此类推，**最后 $n\bmod k$ 个珠子不会组成项链，而是被丢弃**。

现在让你求出一个 $k$ 值，使得在 $\left\lfloor\dfrac{n}{k}\right\rfloor$ 个项链 $b$ 中，存在 **不同的** 项链数量最多。

项链可以反转，形式化地，$b_x$ 和 $b_y$ 不同，当且仅当存在至少一个 $i$，使得 $b_{x,i}\ne b_{y,i}$ 且 $b_{x,i} \ne b_{y,k-i+1}$。

例如 $[1,2,3]$ 和 $[3,2,1]$ 是相同的，而 $[1,2,3]$ 和 $[2,3,1]$ 是不同的。

### 【输入格式】

输入两行，第一行为 $n$。

第二行为 $n$ 个正整数，第 $i$ 个正整数代表 $a_i$。

### 【输出格式】

输出两行。

第一行两个整数，分别代表不同的项链最多的数量，以及不同的项链最多时，$k$ 的个数。

第二行若干个整数，代表所有能使不同的项链最多的 $k$ 值，这可以按任意顺序输出。

### 【样例解释】

$a$ 为 $[1,1,1,2,2,2,3,3,3,1,2,3,3,1,2,2,1,3,3,2,1]$。

- $k=1$ 的时候，我们得到 $3$ 个不同的项链 $b$：$[1],[2],[3]$。
- $k=2$ 的时候，我们得到 $6$ 个不同的项链：$[1,1],[1,2],[2,2],[2,3],[3,3],[3,1]$。
- $k=3$ 的时候，我们得到 $5$ 个不同的项链：$[1,1,1],[2,2,2],[3,3,3],[1,2,3],[3,1,2]$。
- $k=4$ 的时候，我们得到 $5$ 个不同的项链：$[1,1,1,2],[2,2,3,3],[3,1,2,3],[3,1,2,2],[1,3,3,2]$。

### 【数据范围】

对于全部数据，$1\le n\le2\times 10^5$，且 $\forall 1\le i\le n$，有 $1\le a_i\le n$。

```input1
21
1 1 1 2 2 2 3 3 3 1 2 3 3 1 2 2 1 3 3 2 1
```

```output1
6 1
2
```

## 提示
$1≤n≤2\times 10^5$，且 $\forall 1\le i\le n$，有 $1\le a_i\le n$

