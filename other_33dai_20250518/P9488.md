## 题目描述
ZHY 有一个 $n$ 个点的完全图，点 $u$ 与点 $v$ 的距离为 $\gcd(u,v)$，求这个完全图的最大生成树的边权之和。

## 输入格式
一个正整数 $n$。

## 输出格式
一个整数，表示这个最大生成树的边权之和。

```input1
4
```

```output1
4
```

```input2
30
```

```output2
183
```

```input3
100
```

```output3
1916
```

## 提示
**本题采用捆绑测试。**

$\text{Subtask}$ $0\kern{3pt}$(10pts)：$n\le 5$。

$\text{Subtask}$ $1\kern{3pt}$(20pts)：$n\le 1000$。

$\text{Subtask}$ $2\kern{3pt}$(30pts)：$n\le 10^{6}$。

$\text{Subtask}$ $3\kern{3pt}$(40pts)：$n\le 10^{7}$。

对于所有测试数据，$1\le n \le 10^{7}$。

