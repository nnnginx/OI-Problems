# AT_abc288_e [ABC288E] Wish List

## 题目描述

商店里有 $N$ 件商品，标号 $1\sim N$，第 $i$ 件商品有**底价** $A_i$ 且只有一件。

Takahashi 想要买其中的 $M$ 件商品，分别是标号 $X_1,X_2,\ldots,X_M$ 的商品。

他会按照以下的方式买东西：

若还剩 $r$ 件商品没有购买过，选择一个符合 $1\le j\le r$ 的 $j$，付这件商品的底价加上 $C_j$ 的钱购买其中标号第 $j$ 小的商品。

求出买到它想要的商品所付的最小价钱。

注意他也可以买不想要的商品。

## 输入格式

第一行两个正整数 $N$ 和 $M$（$1\le M\le N\le 5000$）表示物品数量和想要的物品数量。

第二行 $n$ 个正整数表示 $A$ 数组（$1\le A_i\le 10^9$）。

第三行 $n$ 个正整数表示 $C$ 数组（$1\le C_i\le 10^9$）。

第四行 $m$ 个正整数表示 $X$ 数组（$1\le X_1 < X_2 < \ldots < X_M\le N$）。

## 输出格式

一行一个正整数表示答案。

### 样例解释

样例 $1$ 中，下面是一种可行的方法：

- 一开始有标号为 $1,2,3,4,5$ 的物品。选择 $j = 5$，购买标号第 $5$ 小的物品（即物品 $5$），付 $A_5 + C_5 = 8$ 的钱；

- 此时有标号为 $1,2,3,4$ 的物品。选择 $j = 2$，购买标号第 $2$ 小的物品（即物品 $2$），付 $A_2 + C_2 = 3$ 的钱；

- 最后有标号为 $1,3,4$ 的物品。选择 $j = 2$，购买标号第 $2$ 小的物品（即物品 $3$），付 $A_3 + C_2 = 6$ 的钱。

Takahashi 现在买到了想要的物品（$3$ 和 $5$）以及一个不想要的物品 $2$，付了最少的 $8+3+6 = 17$ 的钱。

## 输入输出样例 #1

### 输入 #1

```
5 2
3 1 4 1 5
9 2 6 5 3
3 5
```

### 输出 #1

```
17
```

## 输入输出样例 #2

### 输入 #2

```
20 8
29 27 79 27 30 4 93 89 44 88 70 75 96 3 78 39 97 12 53 62
32 38 84 49 93 53 26 13 25 2 76 32 42 34 18 77 14 67 88 12
1 3 4 5 8 14 16 20
```

### 输出 #2

```
533
```