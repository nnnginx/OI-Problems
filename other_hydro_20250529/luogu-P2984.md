## 题目描述
Farmer John is distributing chocolates at the barn for Valentine's day, and $B$ ($1 \le B \le 25000$) of his bulls have a special cow in mind to receive a chocolate gift.

Each of the bulls and cows is grazing alone in one of the farm's $N$ ($2\times B \le N \le 50000$) pastures conveniently numbered $1\dots N$ and connected by $M$ ($N-1 \le M \le 10^5$) bidirectional cowpaths of various lengths. Some pastures might be directly connected by more than one cowpath. Cowpath $i$ connects pastures $R_i $ and $S_i$ ($1 \le R_i \le N$; $1 \le S_i \le N$) and has length $L_i$ ($1 \le L_i \le 2000$).

Bull $i$ resides in pasture $P_i$ ($1 \le P_i \le N$) and wishes to give a chocolate to the cow in pasture $Q_i$ ($1 \le Q_i \le N$).

Help the bulls find the shortest path from their current pasture to the barn (which is located at pasture $1$) and then onward to the pasture where their special cow is grazing. The barn connects, one way or another (potentially via other cowpaths and pastures) to every pasture.

As an example, consider a farm with $6$ pastures, $6$ paths, and $3$ bulls (in pastures $2$, $3$, and $5$) who wish to bestow chocolates on their love-objects:

```cpp

                      *1  <-- Bull wants chocolates for pasture 1 cow
             [4]--3--[5]  <-- [5] is the pasture ID
            /  |
           /   |
          4    2          <-- 2 is the cowpath length
         /     |               between [3] and [4]
      [1]--1--[3]*6
     /   \    /
    9     3  2
   /       \/
 [6]      [2]*4
```
\* The Bull in pasture $2$ can travel distance $3$ (two different ways) to get to the barn then travel distance $2+1$ to pastures $[3]$ and $[4]$ to gift his chocolate. That's $6$ altogether.

\* The Bull in pasture $5$ can travel to pasture $4$ (distance $3$), then pastures $3$ and $1$ (total: $3 + 2 + 1 = 6$) to bestow his chocolate offer.

\* The Bull in pasture $3$ can travel distance $1$ to pasture $1$ and then take his chocolate $9$ more to pasture $6$, a total distance of $10$.

## 输入格式
\* Line $1$: Three space separated integers: $N$, $M$, and $B$;

\* Lines $2\dots M+1$: Line $i+1$ describes cowpath $i$ with three space-separated integers: $R_i$, $S_i$, and $L_i$;

\* Lines $M+2\dots M+B+1$: Line $M+i+1$ contains two space separated integers: $P_i$ and $Q_i$.

## 输出格式
\* Lines $1\dots B$: Line $i$ should contain a single integer, the smallest distance that the bull in pasture $P_i$ must travel to get chocolates from the barn and then award them to the cow of his dreams in pasture $Q_i$.

## 题目大意
### 题目描述

FJ 有 $B$ 头奶牛 $(1\le B\le 25000)$，有 $N(2\times B\le N\le 50000)$ 个农场，编号 $1$ 到 $N$，有 $M(N-1\le M\le 100000)$ 条双向边，第 $i$ 条边连接农场 $R_i$ 和 $S_i(1\le R_i\le N, 1\le S_i\le N)$，该边的长度是 $L_i(1\le L_i\le 2000)$。居住在农场 $P_i$ 的奶牛 A $(1\le P_i\le N)$，想送一份新年礼物给居住在农场 $Q_i(1\le Q_i\le N)$ 的奶牛 B，但是奶牛 A 必须先到 FJ（居住在编号 $1$ 的农场）那里取礼物，然后再送给奶牛 B。你的任务是：奶牛 A 至少需要走多远的路程？

### 输入格式
* 第一行三个整数 $N,M,B$。
* 第 $2$ 至 $M+1$ 行，每行 $3$ 个整数 $R_i,S_i,L_i$。

* 第 $M+2$ 至 $M+B+1$ 行，进行 $B$ 次询问，每行 $2$ 个整数 $P_i ,Q_i$。

### 输出格式
每次询问输出一个整数，即答案。


```input1
6 7 3 
1 2 3 
5 4 3 
3 1 1 
6 1 9 
3 4 2 
1 4 4 
3 2 2 
2 4 
5 1 
3 6 

```

```output1
6 
6 
10 

```

