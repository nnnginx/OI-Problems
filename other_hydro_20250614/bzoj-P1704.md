## 题目描述
农夫约翰有 $n$ 只牛站成一排，有一些很乖的牛朝前站着。但是有些不乖的牛却朝后站着。农夫约翰需要让所有的牛都朝前站着。幸运的是约翰最近买了一个自动转身机。这个神奇的机器能使 $k$ 只连续的牛转身。因为约翰从来都不改变 $k$ 的价值，请帮助他求出 $k$，使旋转次数 $m$ 达到最小。同时要求出对应的 $m$。
## 输入格式
 第一行：整数 $n$。  
 第二行到第 $n+1$ 行：第 $i+1$ 行表示牛 $i$ 的朝向，`F` 表示朝前，`B` 表示朝后。
## 输出格式
 一行两个数，分别是 $k$ 和 $m$，中间用空格隔开。

```input1
7
B
B
F
B
F
B
B
```
```output1
3 3
```
## 样例说明

INPUT DETAILS:  
There are seven cows and they are facing backward, backward, forward, backward, forward, backward, and backward, respectively.

OUTPUT DETAILS:  
For $k = 3$, the machine must be operated three times: turn cows $(1,2,3)$,$(3,4,5)$, and finally $(5,6,7)$:
```
 B > F   F   F
 
 B > F   F   F
 
 F > B > F   F
 
 B   B > F   F
 
 F   F > B > F
 
 B   B   B > F
 
 B   B   B > F
```
## 提示
当 $k=3$ 时神奇的机器旋转 $3$ 次：$(1,2,3),(3,4,5)$ 和 $(5,6,7)$。
## 数据规模与约定
对于 $100\%$ 的数据，$1\le k\le n\le 5\times 10^3$。
## 题目来源
Gold