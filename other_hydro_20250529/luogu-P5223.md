## 题目背景
${\rm CYJian}$最近想起了[水の三角](https://www.luogu.org/problemnew/show/P5014)，他觉得太水了，于是想了一个更加有意思的版本。

## 题目描述
给你$N$和$K$，请你求出：

$$\sum_{i=1}^{K}f[N][i] \ (\bmod\ 998244353)$$

其中：

$$f[i][j]=f[i-1][j]+f[i][j-1]+f[i-1][j-1](i>1,j \leq i)$$

$$f[1][1] = 1 \qquad f[i][0] = 0 \qquad f[i][j]=0(j>i)$$

## 输入格式
第一行两个正整数表示$N$，$K$。

## 输出格式
一行，输出上面式子的值。

```input1
1 1
```

```output1
1

```

```input2
2 2

```

```output2
3

```

```input3
3 3

```

```output3
11

```

```input4
4 3

```

```output4
23

```

## 提示
对于$10\%$的数据：$1 \leq N \leq 10^3 \qquad 1 \leq K \leq 10^2$

对于$30\%$的数据：$1 \leq N \leq 10^6 \qquad 1 \leq K \leq 10^2$

对于$50\%$的数据：$1 \leq N \leq 10^{18} \qquad 1 \leq K \leq 10^2$

对于另$20\%$的数据：$1 \leq N \leq 10^6 \qquad 1 \leq K \leq 10^3$

对于$100\%$的数据：$1 \leq N \leq 10^{18} \qquad 1 \leq K \leq 10^3$

保证$K \leq N$

Upd：时限改为了：第$1$~$35$的测试点时限为$600ms$，第$36$~$50$的测试点时限为$400ms$。

