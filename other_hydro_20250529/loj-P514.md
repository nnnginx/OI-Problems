## 题目描述


给定一个长度为 $n$ 的序列 $A$ 。

定义 $f(l,r)=\sum_{i=l}^{r} A_{i}$。

询问 $m$ 次，每次询问一个数字 $x$，请求出所有满足 $r-l+1 \ge x$ 区间 $[l,r]$ 中最大的 $f(l,r)$。

## 输入格式

第一行两个数，表示 $n$ 和 $m$ 。   
之后 $n$ 个数，表示序列 $A$。    
之后 $m$ 行每行一个数 $x$，表示询问 $x$ 。

## 输出格式

输出 $m$ 行，每行一个答案，表示最大的 $f(l,r)$ 。

```input1
5 5
1 2 3 4 5
1
2
3
4
5
```

```output1
15
15
15
15
15
```

## 数据范围与提示

$1 \leq x \leq n \leq 10^{4}$ ，$0 \leq m \leq 10^{5}$ ， $|A_i| \leq 10^{4}$ 。

