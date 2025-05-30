## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc106/tasks/arc106_d

長さ $ N $ の整数列 $ A\ =\ (A_1,\ A_2,\ \cdots,\ A_N) $ と整数 $ K $ が与えられます。

$ 1\ \le\ X\ \le\ K $ を満たす整数 $ X $ それぞれについて、以下の値を求めてください。

$ \left(\displaystyle\ \sum_{L=1}^{N-1}\ \sum_{R=L+1}^{N}\ (A_L+A_R)^X\right)\ \bmod\ 998244353 $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式
$ K $ 行出力せよ。

$ X $ 行目には、$ \left(\displaystyle\ \sum_{L=1}^{N-1}\ \sum_{R=L+1}^{N}\ (A_L+A_R)^X\ \right)\ \bmod\ 998244353 $ の値を出力せよ。

## 题目大意
给定长度为 $n$ 的序列 $a$，以及一个整数 $k$。

对于每个 $1\le x \le k$，求出如下式子的值：
$$\sum_{l=1}^{n-1}\sum_{r=l+1}^n \left(a_l + a_r\right)^ x$$

答案对 $998244353$ 取模。

$2\le n \le 2\times 10^5,\ 1 \le k \le 300, \ 1\le a_i \le 10^8$。

```input1
3 3
1 2 3
```

```output1
12
50
216
```

```input2
10 10
1 1 1 1 1 1 1 1 1 1
```

```output2
90
180
360
720
1440
2880
5760
11520
23040
46080
```

```input3
2 5
1234 5678
```

```output3
6912
47775744
805306038
64822328
838460992
```

## 提示
### 制約

- 入力は全て整数
- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ K\ \le\ 300 $
- $ 1\ \le\ A_i\ \le\ 10^8 $

### Sample Explanation 1

$ 1 $ 行目には、$ (1+2)^1\ +\ (1+3)^1\ +\ (2+3)^1\ =\ 3\ +\ 4\ +\ 5\ =\ 12 $ を出力します。 $ 2 $ 行目には、$ (1+2)^2\ +\ (1+3)^2\ +\ (2+3)^2\ =\ 9\ +\ 16\ +\ 25\ =\ 50 $ を出力します。 $ 3 $ 行目には、$ (1+2)^3\ +\ (1+3)^3\ +\ (2+3)^3\ =\ 27\ +\ 64\ +\ 125\ =\ 216 $ を出力します。

### Sample Explanation 3

$ \bmod\ 998244353 $ での値を出力してください。

