# AT_arc145_e [ARC145E] Adjacent XOR

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc145/tasks/arc145_e

長さ $ N $ の非負整数列 $ A=(A_1,A_2,\ldots,A_{N}),B=(B_1,B_2,\ldots,B_{N}) $ が与えられます。

数列 $ A $ に対し以下の操作を $ 70000 $ 回以下行うことで $ A $ を $ B $ に一致させられるか判定し、可能な場合は実際に操作手順を一つ示してください。

- 整数 $ K\ (1\le\ K\ \le\ N) $ を選ぶ。全ての $ i\ (2\leq\ i\ \leq\ K) $ について、$ A_i $ の値を $ A_{i-1}\ \oplus\ A_i $ で置き換える。この置き換えは全ての $ i\ (2\leq\ i\ \leq\ K) $ に対して同時に行う。

ただしここで、$ \oplus $ はビット単位 $ \mathrm{XOR} $ 演算を表します。

 ビット単位 $ \mathrm{XOR} $ 演算とは非負整数 $ A,B $ のビット単位 $ \mathrm{XOR} $ 演算、$ A\oplus\ B $ は、以下のように定義されます。

- $ A\oplus\ B $ を二進表記した際の $ 2^k\ (k\geq\ 0) $ の位の数は、$ A,B $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。

例えば、$ 3\oplus\ 5\ =\ 6 $ となります（二進表記すると: $ 011\oplus\ 101\ =\ 110 $)。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $ $ B_1 $ $ B_2 $ $ \ldots $ $ B_N $

## 输出格式

$ 70000 $ 回以下の操作で $ A $ を $ B $ に一致させられない場合、`No` と出力せよ。一致させられる場合、操作回数を $ M $ 回とし、$ i $ 回目の操作で選んだ整数を $ K_i $ として以下の形式で出力せよ。

> Yes $ M $ $ K_1 $ $ K_2 $ $ \ldots $ $ K_M $

条件を満たす解が複数存在する場合、どれを出力しても正解とみなされる。

## 输入输出样例 #1

### 输入 #1

```
3
1 2 0
1 2 3
```

### 输出 #1

```
Yes
2
2 3
```

## 输入输出样例 #2

### 输入 #2

```
2
10 100
1 0
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
2
1152921504606846975 0
1152921504606846975 0
```

### 输出 #3

```
Yes
0
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 1000 $
- $ 0\ \leq\ A_i,\ B_i\ <\ 2^{60} $
- 入力は全て整数

### Sample Explanation 1

この出力例では、操作によって数列 $ A $ は以下のように変化します。 - 初期状態：$ A=(1,\ 2,\ 0) $ - $ 1 $ 回目の操作後：$ A=(1,\ 3,\ 0) $ - $ 2 $ 回目の操作後：$ A=(1,\ 2,\ 3) $ $ 2 $ 回の操作後、$ A $ と $ B $ は一致しているのでこの出力は条件を満たします。