# AT_abc236_e [ABC236E] Average and Median

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

## 输入输出样例 #1

### 输入 #1

```
6
2 1 2 1 1 10
```

### 输出 #1

```
4
2
```

## 输入输出样例 #2

### 输入 #2

```
7
3 1 4 1 5 9 2
```

### 输出 #2

```
5.250000000
4
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^{9} $
- 入力は全て整数である。

### Sample Explanation 1

$ 2 $ 番目、$ 4 $ 番目、$ 6 $ 番目のカードを選ぶと、書かれた整数の平均は $ \frac{12}{3}\ =\ 4 $ となり、これが最大です。 $ 1 $ 番目、$ 3 $ 番目、$ 5 $ 番目、$ 6 $ 番目のカードを選ぶと、書かれた整数の中央値は $ 2 $ となり、これが最大です。

### Sample Explanation 2

平均値の出力については誤差が認められるので、例えば $ 5.2491 $ と出力しても正答とみなされます。ただし、中央値は正確な値を出力しなければなりません。