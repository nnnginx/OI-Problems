## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc120/tasks/arc120_a

数列 $ a\ =\ (a_1,\ a_2,\ a_3,\ \dots,\ a_k) $ に対して、$ f(a) $ を、以下の操作を行った後の $ a $ の要素の総和と定義します。

- $ i\ =\ 1,\ 2,\ 3,\ \dots,\ k $ の順に以下の操作を行う :  
   現在の $ a $ の要素の最大値を $ a_i $ に足す

長さ $ N $ の数列 $ A\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_N) $ が与えられます。  
 $ 1 $ 以上 $ N $ 以下の各整数 $ k $ について、$ a\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_k) $ としたときの $ f(a) $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ $ \dots $ $ A_N $

## 输出格式
$ N $ 行にわたって出力せよ。$ k $ 行目には $ a\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_k) $ としたときの $ f(a) $ を出力せよ。

## 题目大意
## 题目翻译

对于一个数列 $a = (a_1, a_2, a_3, \dots, a_k)$，让 $f(a)$ 成为它的元素之和，在完成下列操作之后：

- 对于每个 $i = 1, 2, 3, \dots, k$，依次进行以下操作：
    将$a$中某元素的当前最大值加到 $a_i$ 中。

给你一个长度为$N$的序列：$A = (A_1, A_2, A_3, \dots, A_N)$。
对于介于 $1$ 和 $N$（含）之间的每个整数 $k$，求当 $a = (A_1, A_2, A_3, \dots， A_k)$ 时的 $f(a)$。

```input1
3
1 2 3
```

```output1
2
8
19
```

## 提示
### 制約

- $ 1\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ A_i\ \le\ 10^7 $
- 入力に含まれる値は全て整数

### Sample Explanation 1

例えば $ a\ =\ (A_1,\ A_2,\ A_3) $ のときの $ f(a) $ は以下のように計算されます。 - まず $ i\ =\ 1 $ として、現在の $ a $ の最大値である $ 3 $ を $ a_1 $ に足す。$ a\ =\ (4,\ 2,\ 3) $ となる。 - 次に $ i\ =\ 2 $ として、現在の $ a $ の最大値である $ 4 $ を $ a_2 $ に足す。$ a\ =\ (4,\ 6,\ 3) $ となる。 - 最後に $ i\ =\ 3 $ として、現在の $ a $ の最大値である $ 6 $ を $ a_3 $ に足す。$ a\ =\ (4,\ 6,\ 9) $ となる。 - 操作後の $ a $ の総和である $ 19 $ が $ f(a) $ の値である。

