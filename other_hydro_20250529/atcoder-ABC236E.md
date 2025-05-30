## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc236/tasks/abc236_e

$ N $ 枚のカードがあり、$ i\ \,\ (1\ \leq\ i\ \leq\ N) $ 番目のカードには整数 $ A_i $ が書かれています。

高橋君は、これらのカードから好きな枚数選びます。ただし、各 $ i\ \,\ (1\ \leq\ i\ \leq\ N\ -\ 1) $ について、$ i $ 番目のカードと $ i\ +\ 1 $ 番目のカードの少なくとも一方を選ぶ必要があります。

以下の値を求めてください。

- 選んだカードに書かれた整数の平均値としてあり得る最大値
- 選んだカードに書かれた整数の中央値としてあり得る最大値

ただし、$ n $ 個の整数の中央値は、それらのうち小さい方から数えて $ \lceil\ \frac{n}{2}\ \rceil $ 番目であるものとします。ここで、$ \lceil\ x\ \rceil $ は $ x $ 以上の最小の整数を表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式
$ 2 $ 行出力せよ。$ 1 $ 行目には選んだカードに書かれた整数の平均値としてあり得る最大値を、$ 2 $ 行目には選んだカードに書かれた整数の中央値としてあり得る最大値を出力せよ。 平均値の出力については、正しい値との相対誤差または絶対誤差が $ 10^{-3} $ 以下であれば正答とみなされる。

## 题目大意
$n$ 个数 $a_{1}\dots a_n$ 排成一列。现在要选出一些数，满足 **任意两个相邻的数中至少有一个数被选择**。

请求出：

- 所有选择方案中，被选中的数字平均值的最大值，误差在 $10^{-3}$ 以内视为正确；

- 所有选择方案中，被选中的数字中位数的的最大值。在这里，偶数 $2k$ 个数的中位数视作第 $k$ 小的数。

- $2\leq n\leq 10^5$

- $1\leq a_i\leq 10^9$

```input1
6
2 1 2 1 1 10
```

```output1
4
2
```

```input2
7
3 1 4 1 5 9 2
```

```output2
5.250000000
4
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^{9} $
- 入力は全て整数である。

### Sample Explanation 1

$ 2 $ 番目、$ 4 $ 番目、$ 6 $ 番目のカードを選ぶと、書かれた整数の平均は $ \frac{12}{3}\ =\ 4 $ となり、これが最大です。 $ 1 $ 番目、$ 3 $ 番目、$ 5 $ 番目、$ 6 $ 番目のカードを選ぶと、書かれた整数の中央値は $ 2 $ となり、これが最大です。

### Sample Explanation 2

平均値の出力については誤差が認められるので、例えば $ 5.2491 $ と出力しても正答とみなされます。ただし、中央値は正確な値を出力しなければなりません。

