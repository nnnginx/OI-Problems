## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc103/tasks/abc103_c

$ N $ 個の正整数 $ a_1,\ a_2,\ ...,\ a_N $ が与えられます。

非負整数 $ m $ に対して、$ f(m)\ =\ (m\ mod\ a_1)\ +\ (m\ mod\ a_2)\ +\ ...\ +\ (m\ mod\ a_N) $ とします。

ここで、$ X\ mod\ Y $ は $ X $ を $ Y $ で割った余りを表します。

$ f $ の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式
$ f $ の最大値を出力せよ。

## 题目大意
输入 $N$ 和 $a_1,a_2,\ldots,a_N$。

令 $f(m)=(m\bmod a_1)+(m\bmod a_2)+\ldots+(m\bmod a_N)$

问 $f(m)$ 最大是多少（$m$ 可为任意整数）。

其中 $2\le N\le 3000,2\le a_i\le 10^5$。

```input1
3
3 4 6
```

```output1
10
```

```input2
5
7 46 11 20 11
```

```output2
90
```

```input3
7
994 518 941 851 647 2 581
```

```output3
4527
```

## 提示
### 制約

- 入力は全て整数である
- $ 2\ \leq\ N\ \leq\ 3000 $
- $ 2\ \leq\ a_i\ \leq\ 10^5 $

### Sample Explanation 1

$ f(11)\ =\ (11\ mod\ 3)\ +\ (11\ mod\ 4)\ +\ (11\ mod\ 6)\ =\ 10 $ が $ f $ の最大値です。

