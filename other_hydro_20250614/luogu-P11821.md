## 题目背景
P11817 的加强版。本题存在 $\Theta(\sqrt n\log n)$ 的做法。

本题数据为自造。

std: joke3579，validator & generator: Starrykiller。

**请勿提交 OEIS 题解。**



## 题目描述
求出 $n$ 个节点的满足以下条件的**有标号有向简单图**的数量：

- $\forall 1\le i\le n$，$\operatorname{deg_{out}}(i)=\operatorname{deg_{in}}(i)=2$。

这里，$\operatorname{deg_{out}}(u)$ 指节点 $u$ 的出度，$\operatorname{deg_{in}}(u)$ 指节点 $u$ 的入度。

你只需要输出答案对给定大素数 $p$ 取模后的结果。


注意我们是对**有标号**的「有向简单图」计数。也就是说，这张图中无重边自环。注意 $u\to v$ 和 $v\to u$ 同时出现是允许的。




## 输入格式
一行两个正整数 $n,p$。

## 输出格式
一行一个非负整数，表示答案。

```input1
4 998244853
```

```output1
9
```

```input2
114514 1000000007

```

```output2
637348702

```

## 提示
- $3\le n\le 10^7$；
- $10^8+7\le p\le 10^9+7$，$p$ 为素数。



