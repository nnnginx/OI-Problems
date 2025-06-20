# AT_abc270_h [ABC270Ex] add 1

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc270/tasks/abc270_h

$ A_1=0 $ かつ $ A_N\ >\ 0 $ であるような、$ N $ 個の非負整数の組 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。

高橋君は $ N $ 個のカウンターを持っており、最初、全てのカウンターの値は $ 0 $ です。  
高橋君は、全ての $ 1\leq\ i\leq\ N $ について $ i $ 番目のカウンターの値が $ A_i $ 以上となるまで次の操作を繰り返します。

> $ N $ 個のカウンターの中から $ 1 $ つを等確率に選び、その値を $ 0 $ にする。（選択は毎回独立に行う。）  
> 選んだカウンター **以外** のカウンターの値を $ 1 $ 増加させる。

高橋君の操作回数の期待値を $ \mathrm{mod} $ $ 998244353 $ で出力してください（注記参照）。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

高橋君の操作回数の期待値を $ \mathrm{mod} $ $ 998244353 $ で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
0 2
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
5
0 1 3 10 1000000000000000000
```

### 输出 #2

```
874839568
```

## 说明/提示

### 注記

求める期待値は必ず有限値かつ有理数となることが証明できます。また、この問題の制約下では、その値を互いに素な $ 2 $ つの整数 $ P $, $ Q $ を用いて $ \frac{P}{Q} $ と表したとき、$ R\ \times\ Q\ \equiv\ P\pmod{998244353} $ かつ $ 0\ \leq\ R\ \lt\ 998244353 $ を満たす整数 $ R $ がただ一つ存在することが証明できます。この $ R $ を求めてください。

### 制約

- $ 2\leq\ N\leq\ 2\times\ 10^5 $
- $ 0=A_1\leq\ A_2\leq\ \cdots\ \leq\ A_N\leq\ 10^{18} $
- $ A_N\ >\ 0 $
- 入力は全て整数

### Sample Explanation 1

$ i $ 番目のカウンターの値を $ C_i $ で表します。 高橋君の操作が終了するまでの一連の流れの例は次の通りです。 - $ 1 $ 番目のカウンターの値を $ 0 $ にした後、それ以外のカウンターの値を $ 1 $ 増加させる。 $ (C_1,C_2)=(0,1) $ となる。 - $ 2 $ 番目のカウンターの値を $ 0 $ にした後、それ以外のカウンターの値を $ 1 $ 増加させる。 $ (C_1,C_2)=(1,0) $ となる。 - $ 1 $ 番目のカウンターの値を $ 0 $ にした後、それ以外のカウンターの値を $ 1 $ 増加させる。 $ (C_1,C_2)=(0,1) $ となる。 - $ 1 $ 番目のカウンターの値を $ 0 $ にした後、それ以外のカウンターの値を $ 1 $ 増加させる。 $ (C_1,C_2)=(0,2) $ となる。 この場合の操作回数は $ 4 $ となります。 $ 1,2,3,4,5,\ldots $ 回で操作が終了する確率はそれぞれ $ 0,\frac{1}{4},\ \frac{1}{8},\ \frac{1}{8},\ \frac{3}{32},\ldots $ であり、 期待値は $ 2\times\frac{1}{4}+3\times\frac{1}{8}+4\times\frac{1}{8}+5\times\frac{3}{32}+\dots=6 $ となります。 よって、 $ 6 $ を出力します。