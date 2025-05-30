## 题目背景

小明这天正在做题，题目中有很多变量，并有一些特殊的公式描述了变量间的关系，小明想要利用这些关系求解变量的值。

每一个公式描述且仅描述了两个变量之间的关系，规则如下：

- 当我们知道了变量 $A$ 和变量 $B$ 之间的关系后，如果又知道了变量 $A$ 和变量 $C$ 之间的关系，我们即可推导出变量 $B$ 和变量 $C$ 之间的关系。

- 当我们同时知道变量 $A$ 和变量 $B$ 之间的两个不同的关系，我们就能推导出变量 $A$ 和变量 $B$ 的值。

- 当我们已经知道变量 $A$ 的值，同时又知道变量 $A$ 和变量 $B$ 之间的关系，我们就能推导出变量 $B$ 的值。

现在小明不断地加入公式，你能告诉他每次加入一个公式后，有多少变量的值可以被推导出吗？

## 输入格式

第一行两个数 $n,~m$，表示有 $n$ 个变量和 $m$ 条公式。

接下来 $m$ 行，每行两个整数 $x,~y$，表示了一个公式，这条公式描述了 $x$ 号变量和 $y$ 号变量之间的关系。（可能重复）

## 输出格式

输出 $m$ 行，每行一个整数，表示加入前 $i$ 号公式后能够推导出的变量的数量。

```input1
5 5
1 2
2 3
1 2
3 4
4 5
```

```output1
0
0
3
4
5
```

```input2
5 5
1 2
1 2
3 4
4 5
2 5
```

```output2
0
2
2
2
5
```

## 提示说明

对于 $10\%$ 的数据，$1 \le n \le 10,~1 \le m \le 20,~1 \le x,y \le n$。

对于 $50\%$ 的数据，$1 \le n \le 10^3,~1 \le m \le 2\times10^3,~1 \le x,y \le n$。

对于 $100\%$ 的数据，$1 \le n \le 10^5,~1 \le m \le 2\times10^5,~1 \le x,y \le n$。