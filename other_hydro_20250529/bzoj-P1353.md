## 题目描述

给出一个平行四边形的长与高。给出入口与出口。

对于四边形的每条边都有一种 $\rm{Color}$，非黑即白。

你要找出一条路径，走过的边黑白交替，且长度最短。

## 输入格式

第一行给出平行四边形的长 $n$ 与高 $m$。

第二行给出入口，出口坐标。

下面的字符矩阵代表这个平行四边形每条边的 $\rm{Color}$。

## 输出格式

输出路径的最少长度。


```input1
2 1
0 0 2 1
bb
nwwnw
bn
```



```output1
6
```



```input2
5 4
0 2 5 2
nnbnn
nnnwwbwnnnn
nbbbn
nnwbwwbwwnn
bwwww
nnbwbbwwbnn
nwwwn
nnnnbwbbnnn
nnwnn
```



```output2
22
```

## 数据规模与约定

对于 $100\%$ 的数据，满足 $1\leq n,m\leq 500$。

## 提示

对于第一个数据: $(0, 0) \rightarrow (1, 0) \rightarrow (0, 1) \rightarrow (1, 1) \rightarrow (1, 0) \rightarrow (2, 0) \rightarrow (2, 1) $。

对于第二个数据: $(0, 2) \rightarrow (1, 2) \rightarrow (1, 1) \rightarrow (2, 1) \rightarrow (2, 0) \rightarrow (3, 0) \rightarrow (3, 1) \rightarrow (3, 2) \rightarrow (4, 1) \rightarrow (3, 1) \rightarrow (3, 0) \rightarrow (2, 0) \rightarrow (2, 1) \rightarrow (1, 1) \rightarrow (1, 2) \rightarrow (1, 3) \rightarrow (2, 3) \rightarrow (2, 4) \rightarrow (3, 4) \rightarrow (3, 3) \rightarrow (4, 3) \rightarrow (4, 2) \rightarrow (5, 2)$。