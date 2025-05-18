## 题目背景
本题是[「Stoi2031」兰亭序](https://www.luogu.com.cn/problem/P7487) 的加强版。

## 题目描述
给定 $n=a^b,k$，对 $1 \le t \le k$ 求

$$\prod_{x_1=1}^{n}\prod_{x_2=1}^{n}\dots\prod_{x_t=1}^{n}\left( 1+e^{\frac{2\pi ix_1x_2\dots x_t}{n}} \right) \bmod{335544323}$$

输出所有 $k$ 个答案的异或和。

其中 $e^{it}=\cos{t}+i\sin{t}$ 对所有 $t \in \mathbb{R}$ 成立，$i$ 为虚数单位，满足 $i^2=-1$。

## 输入格式
一行三个正整数 $a,b,k$，其中 $n=a^b$。

## 输出格式
一行一个自然数表示答案。

```input1
15 1 2

```

```output1
201012023

```

```input2
1 7 3

```

```output2
2

```

```input3
3 2 3

```

```output3
301162058

```

```input4
4 2 2

```

```output4
0

```

```input5
19260817 114514 13579

```

```output5
461194421

```

## 提示
对于所有数据，$1 \le a \le 10^{18}$，$1 \le b \le 10^{13}$，$1 \le k \le 10^5$。

