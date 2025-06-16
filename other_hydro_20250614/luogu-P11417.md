## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/p38htsuu.png)

## 题目描述
$f(x)$ 为积性函数，且满足 $f(p^k)=p^{2k}+k$（$p$ 为素数）。

令 $g(x)=\prod\limits_{d|x}f(d)\space \bmod\space (10^9+7)$ ，请计算 $g(i)\space (1\le i \le n)$ 的异或和。

## 输入格式
一行一个正整数 $n$。

## 输出格式
一行一个非负整数。

```input1
5
```

```output1
78
```

```input2
142857
```

```output2
67850062
```

```input3
10000000
```

```output3
505679580
```

## 提示
**本题采用捆绑测试**

| Subtask | n | Score |
| :----------: | :----------: | :----------: |
| $1$ | $\le10^4$ | $10$ |
| $2$ | $\le 5\times 10^6$ | $30$ |
| $3$ | $\le 2\times 10^7$ | $30$ |
| $4$ | $\le 5\times10^7$ | $30$ |

对 $100\%$ 的数据，$1\le n \le 5\times10^{7} $。


