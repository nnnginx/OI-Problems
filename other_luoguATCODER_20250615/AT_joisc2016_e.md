# AT_joisc2016_e サンドイッチ

## 题目描述

你买了 $2nm$块三明治，并将它们拼成了一个$n\times m$ 的矩形。

![](https://cdn.luogu.com.cn/upload/image_hosting/wx6sxi2v.png)

你现在可以选择吃掉一些三明治，每次吃的三明治都必须在边界上。更具体地， 你不能吃掉一块三明治当且仅当以下两个条件同时成立：

1. 这块三明治的斜边与某块未被吃掉的三明治相邻；

2. 这块三明治的至少一条直角边与某块未被吃掉的三明治相邻。

请你求出，对于每个小正方形内的两块三明治，要把它们全部吃掉，至少需要吃多少块三明治(包括这两块三明治)。

## 输入格式

第一行两个整数 $n,m$，表示矩形大小。

接下来 $n$ 行，每行一个长度为 $m$ 的字符串，每个字符为'N'或'Z' 表示这个小矩形内的三明治沿主对角线放置还是沿副对角线放置。

![](https://cdn.luogu.com.cn/upload/image_hosting/30ed6bg6.png)

## 输出格式

输出 $n$ 行每行 $m$ 个整数，第 $i$ 行第 $j$ 个表示对应位置小正方形的答案，若无解则为 $-1$。

## 样例输入1
```
2 3
NZN
ZZN
```
## 样例输出1
```
10 8 2
8 6 4
```
## 样例输入2
```
2 2
NZ
ZN
```
## 样例输出2
```
-1 -1
-1 -1
```
## 样例输入3

```
5 5
NZZZN
NNNZN
NNZNN
NZNNN
NZZZN
```
## 样例输出3
```
10 12 14 16 2
8 -1 -1 -1 4
6 -1 -1 -1 6
4 -1 -1 -1 8
2 16 14 12 10
```

## 说明/提示

对于 $35\%$ 的数据，$n,m\le 50$;

对于所有数据，$1\le n,m\le 400$。