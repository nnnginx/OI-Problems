# AT_s8pc_6_b AtCoder Market

## 题目描述

AtCoder 市场是由 $10^9$ 个方格连成一列的方格来表示的超市。这里，从左数第 $i$ 格被称为第 $i$ 格。

有一天，$n$ 名顾客来到 AtCoder 市场。第 $i$ 个顾客分别购买第 $a_i$ 格和第 $b_i$ 格上的商品。

square1001 君决定在 AtCoder 市场各设置一个入口和出口。入口和出口设置在任意一个方格里。入口和出口可以在同一个地方。

这时，顾客会按照以下路径移动：

首先，从入口开始。通过第 $a_i$ 格和第 $b_i$ 格，在出口到达终点。
对于所有的顾客，在进入相邻方格需要 $1$ 秒。请求出在最佳入口和出口时所有顾客的移动时间总和的最小值。

## 输入格式

第一行，一个正整数 $n$，代表顾客的数量。

接下来 $n$ 行，每行两个数 $a_i$ 和 $b_i$，表示第 $i$ 个顾客分别购买第 $a_i$ 格和第 $b_i$ 格上的商品。

## 输出格式

输出所有顾客的移动时间总和的最小值。

## 输入输出样例 #1

### 输入 #1

```
3
5 7
2 6
8 10
```

### 输出 #1

```
18
```

## 输入输出样例 #2

### 输入 #2

```
5
1 71
43 64
13 35
14 54
79 85
```

### 输出 #2

```
334
```

## 输入输出样例 #3

### 输入 #3

```
11
15004200 341668840
277786703 825590503
85505967 410375631
797368845 930277710
90107929 763195990
104844373 888031128
338351523 715240891
458782074 493862093
189601059 534714600
299073643 971113974
98291394 443377420
```

### 输出 #3

```
8494550716
```