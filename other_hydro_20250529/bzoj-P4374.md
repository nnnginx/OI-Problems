# 题目描述

利沃夫动物园的小象有 $n$ 个盒子，每个盒子里有一些钱或者钻石。他不知道每个盒子里具体是什么，但他知道如果打开第 $i$ 个盒子，他有 $P_i / 100$ 的概率能获得 $V_i$ 美元的钱，而有 $(1 – P_i / 100)$ 的概率能获得一个钻石。

现在有 $m$ 个物品，分别编号为 $0$ 到 $m-1$ ， 第 $j$ 个物品需要花费恰好 $C_j$ 美元的钱和$D_j$ 个钻石。小象非常聪明，当他获得了一定量的钱和钻石后，他总会买尽可能多的物品。注意，每个物品只能购买一次。现在请你帮助小象计算出，当他打开所有的盒子后，他期望能够买到的物品个数是多少？

# 输入格式

输入的第一行包含一个正整数 $T$，表示数据组数。
对于每组数据，第一行包含两个正整数 $n, m$，分别表示盒子数与物品数。接下来 $n$ 行，每行为两个整数 $V_i, P_i$，分别表示小象能从第 $i$ 个盒子中获得钱的数量与获得钱的概率。接下来 $m$ 行，每行为两个整数 $C_j, D_j$，分别表示第 $j$ 个物品所需要的钱和钻石的数量。

# 输出格式

输出总共 $T$ 行。每行为一个实数，为对应的测试数据的答案，实数四舍五入保留到小数点后 $4$ 位。

```input1
2
2 2
2 50
2 100
2 0
2 0
2 2
2 100
2 50
0 2
0 1

```
```output1
1.5000
0.5000
```

## 提示

1≤T≤5,2≤n≤30,1≤m≤30

1≤Vi, Cj≤107,0≤Dj≤30,0≤Pi≤100

## 题目来源
没有写明来源


