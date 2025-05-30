## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc136/tasks/abc136_e

長さ $ N $ の整数列 $ A_1,\ A_2,\ \cdots,\ A_N $ があります。

次の操作を $ 0 $ 回以上 $ K $ 回以下行うことができます。

- $ i\ \neq\ j $ なる $ 1 $ 以上 $ N $ 以下の $ 2 $ つの整数 $ i,\ j $ を選び、$ A_i $ に $ 1 $ を足し、$ A_j $ に $ -1 $ を足す。この操作の後いずれかの要素が負になってもよい。

操作後の $ A $ の全ての要素を割り切る正の整数として考えられる値の最大値を計算してください。ただし、正の整数 $ x $ が整数 $ y $ を割り切るとは、ある整数 $ z $ を用いて $ y\ =\ xz $ と表せる場合を表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_{N-1} $ $ A_{N} $

## 输出格式
操作後の $ A $ の全ての要素を割り切る正の整数として考えられる値の最大値を出力せよ。

## 题目大意
给定一个长度为 $N$ 的整数序列：$A_1, A_2, \ldots, A_n$。

您可以执行以下操作 $0 \sim K$ 次：

选择两个整数 $i$ 和 $j$，满足 $i \ne j$ 并且 $1 \le i, j \le N$。令 $A_i$ 加上 $1$，令 $A_j$ 减去 $1$，可能产生负的元素。

计算在执行完操作后，整除 $A$ 中每个元素的最大可能正整数。这里正整数 $x$ 整除整数 $y$ 当且仅当存在一个整数 $z$，使得 $y=xz$。

```input1
2 3
8 20
```

```output1
7
```

```input2
2 10
3 5
```

```output2
8
```

```input3
4 5
10 1 2 22
```

```output3
7
```

```input4
8 7
1 7 5 6 8 2 6 5
```

```output4
5
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 500 $
- $ 1\ \leq\ A_i\ \leq\ 10^6 $
- $ 0\ \leq\ K\ \leq\ 10^9 $
- 入力は全て整数である

### Sample Explanation 1

例えば以下の操作で、$ 7 $ が $ A $ の全ての要素を割り切るようにできます。 - $ i\ =\ 2,\ j\ =\ 1 $ とする。$ A $ は $ (7,\ 21) $ となる。 また、$ 8 $ 以上の整数が $ A $ の全ての要素を割り切るようにはできません。

### Sample Explanation 2

例えば、以下のように操作を $ 5 $ 回行います。 - $ i\ =\ 2,\ j\ =\ 1 $ とする。$ A $ は $ (2,\ 6) $ となる。 - $ i\ =\ 2,\ j\ =\ 1 $ とする。$ A $ は $ (1,\ 7) $ となる。 - $ i\ =\ 2,\ j\ =\ 1 $ とする。$ A $ は $ (0,\ 8) $ となる。 - $ i\ =\ 2,\ j\ =\ 1 $ とする。$ A $ は $ (-1,\ 9) $ となる。 - $ i\ =\ 1,\ j\ =\ 2 $ とする。$ A $ は $ (0,\ 8) $ となる。 このとき、$ 0\ =\ 8\ \times\ 0,\ 8\ =\ 8\ \times\ 1 $ と表せるので、$ 8 $ は $ A $ の全ての要素を割り切ります。また、$ 9 $ 以上の整数が $ A $ の全ての要素を割り切るようにはできません。

