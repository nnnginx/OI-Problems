# AT_joisc2017_h 細長い屋敷 (Long Mansion)

## 题目描述

#「JOISC 2017 Day 3」幽深府邸


**题目译自 [JOISC 2017](https://www.ioi-jp.org/camp/2017/2017-sp-tasks/index.html) Day3 T2「[細長い屋敷](https://www.ioi-jp.org/camp/2017/2017-sp-tasks/2017-sp-d3.pdf)（[Long Mansion](https://www.ioi-jp.org/camp/2017/2017-sp-tasks/2017-sp-d3-en.pdf)）」**

$N$ 个房间排列在一条直线上，依次编号为 $1, 2, \ldots, N$。只有编号相邻的房间才相连。相连的房间之间有上锁的门。  
从房间 $i$ 进入房间 $i+1$，或者从房间 $i+1$ 进入房间 $i$，需要类型为 $C_i$ 的钥匙 $(1\le i\le N-1)$。  
进入房间 $i$ 可以捡起房间里的所有钥匙。房间 $i$ 有 $B_i$ 把钥匙，类型分别为 $A[i][1]\dots A[i][B_i]$ 保证对于同一个 $i$，没有两个 $A[i][j]$ 相同。钥匙可以重复使用。你可能会获得相同的钥匙，然并卵。  
现在有 $Q$ 组查询，每组查询用两个整数 $x, y$ 来描述 $(x≠y)$，表示：如果有人被丢进房间 $x$，手上没有任何钥匙，此人能否到达房间 $y$（当然，此人可以捡房间 $x$ 里的钥匙）。  
对于每组查询，如果此人能到达，输出 $\texttt{YES}$，否则输出 $\texttt{NO}$ 。

## 输入格式

第一行有一个整数 $N$。  
第二行有 $N-1$ 个整数 $C_1, C_2, \dots, C_{N-1}$，用空格分隔。  
在接下来的 $N$ 行中，第 $i$ 行 $(1\le i\le N)$ 的开头有一个整数 $B_i$，后面有 $B_i$ 个整数 $A[i][1]\dots A[i][B_i]$，这 $B_i+1$ 个整数用空格分隔。  
第 $N+2$ 行有一个整数 $Q$。  
在接下来的 $Q$ 行中，第 $k$ 行 $(1\le k\le Q)$ 有两个整数 $X_k, Y_k$，表示一组查询。

## 输出格式

输出共 $Q$ 行，每行一个字符串  $\texttt{YES}$ 或 $\texttt{NO}$ ，表示此人能否到达房间 $y$。

## 样例

#### 样例输入 1
```plain
5
1 2 3 4
2 2 3
1 1
1 1
1 3
1 4
4
2 4
4 2
1 5
5 3
```

#### 样例输出 1
```plain
YES
NO
NO
YES
```

#### 样例解释 1
查询 1：可行，此人应依次到 $2, 1, 2, 3, 4$ 号房间搜刮钥匙。  
查询 2：不可行，此人只能到达 $3,4$ 号房间，只能拿到 $1,3$ 号钥匙。  
查询 3：不可行，此人无法拿到 $4$ 号钥匙。  
查询 4：可行，此人应依次到 $5, 4, 3$ 号房间搜刮钥匙。

#### 样例输入 2
```plain
5
2 3 1 3
1 3
1 2
1 1
1 3
1 2
4
1 3
3 1
4 3
2 5
```

#### 样例输出 2
```plain
NO
YES
NO
YES
```

#### 样例输入 3
```plain
7
6 3 4 1 2 5
1 1
1 5
1 1
1 1
2 2 3
1 4
1 6
3
4 1
5 3
4 7
```

#### 样例输出 3
```plain
YES
NO
YES
```

## 说明/提示

对于所有数据，$2\le N\le 5\times 10^5,$ $1\le Q\le 5\times 10^5,$ $1\le \sum B_i \le 5\times 10^5,$ $1\le B_i, C_i, A[i][j], X_k, Y_k\le N,$ $X_k≠Y_k$。

|子任务 #|分值|$N$|$Q$|$\sum B_i$|$C_i, A[i][j]$|
|-|-|-|-|-|-|
|1|5|$N\le 5000$|$Q\le 5000$|$\sum B_i \le 5000$|.|
|2|5|$N\le 5000$|.|$\sum B_i \le 5000$|.|
|3|15|$N\le 10^5$|.|.|$C_i, A[i][j]\le 20$|
|4|75|.|.|.|.|

感谢 Planet6174 提供的翻译