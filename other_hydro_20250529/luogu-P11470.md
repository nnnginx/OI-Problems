## 题目描述
给定一串长度为 $n$ 的数对序列 $(x_i,y_i)$，其中 $x_i, y_i$ 都是整数。

有 $m$ 次询问，每次给定一个两个整数 $a, b$，你需要先选定一个整数 $k$（注意 $k$ 可以为 $0$），然后再选定一个正整数序列 $1 \le p_1 < p_2 < \cdots < p_k \le n$（若 $k = 0$ 则该序列为空），使得
$$
\min\left(a + \sum\limits_{i = 1}^{k} x_{p_i} , b + \sum\limits_{i = 1}^{k} y_{p_i}\right)
$$ 

最大，输出这个最大值。



## 输入格式
第一行一个整数 $n$。

接下来 $n$ 行，每行两个整数代表 $x_i, y_i$。

接下来一行一个整数 $m$。

接下来 $m$ 行，每行两个整数代表每次询问的 $a, b$。

## 输出格式
输出 $m$ 行。

一行一个数字，代表符合题意的最大值。

```input1
2
2 -3
3 -2
1
1 6
```

```output1
4
```

## 提示
$1\le n \le 10^3$，$0\le \sum \lvert x_i\rvert \le 10^5$，$0\le \lvert y_i \rvert \le 10^{12}$，$1\le m \le 2\times 10^5$，$0\le \lvert a\rvert, \lvert b\rvert \le 10^{12}$。

