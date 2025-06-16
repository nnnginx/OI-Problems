# AT_abc236_c [ABC236C] Route Map

## 题目描述

# 题目简述
有 $N$ 个站点按顺序排在一条直线上，第 $i(1\le i\le N)$ 个站点是 $S_i$。

有一辆火车会在其中的 $M(M\le N)$ 个站点停下,第 $j(1\le j\le M)$ 个停下来的站点的名字是 $T_j$。

保证 $T_1=S_1,T_M=S_N$。

对于 $N$ 个站点中的每一个，请判断火车是否在该站点停下。

## 输入格式

第一行包含整数 $N,M$。

第二行包含 $N$ 个字符串 $S_1,S_2,\dots,S_N$。

第三行包含 $M$ 个字符串 $T_1,T_2,\dots,T_M$。

## 输出格式

输出 $N$ 行。如果第 $i(1 \le i \le N)$ 个站点在火车的经停站点列表中，输出 `Yes`，否则输出 `No`。

Translated by @[tianbiandeshenghuo11](/user/752485)

## 输入输出样例 #1

### 输入 #1

```
5 3
tokyo kanda akiba okachi ueno
tokyo akiba ueno
```

### 输出 #1

```
Yes
No
Yes
No
Yes
```

## 输入输出样例 #2

### 输入 #2

```
7 7
a t c o d e r
a t c o d e r
```

### 输出 #2

```
Yes
Yes
Yes
Yes
Yes
Yes
Yes
```

## 说明/提示

>$2≤M≤N≤10^5$
>
>$N,M$ 为整数
>
>$S_i（1 \le i \le N）$是一个长度在 $[1, 10]$ 之间的小写英文字符串。
>
>$S_i\ne S_j（i \ne j）$
>
>$T_1=S_1,T_M=S_N$
>
>$(T_1,\dots, T_M)$ 是通过移除 $(S_1,\dots, S_N)$ 中的若干个站点且不改变原有顺序得到的。