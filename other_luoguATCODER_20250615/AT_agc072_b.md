# AT_agc072_b [AGC072B] AGC Language

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc072/tasks/agc072_b

AGC 語とは、同じ数の `A` と `C` のみからなり、どの接頭辞についても `A` が半数以上を占める $ 2 $ 文字以上の文字列を指します。 $ N $ 個の `A` と $ N $ 個の `C` からなる $ 2N $ 文字の文字列 $ S $ が与えられるので、$ k\ =\ 1,\ 2,\ \dots,\ K $ について次の問いに答えてください。

> 黒板に $ S $ を $ k $ 回繰り返した文字列が書かれている。 以下の操作をその順に行うことで、黒板の文字列を AGC 語にしたい。
> 
> 1. 次の操作を **1 回だけ**行う。
>   - 整数 $ (l,\ r) $ $ (1\ \leq\ l\ \leq\ r\ \leq\ 2kN) $ を選択し、文字列の $ l $ から $ r $ 文字目までの部分を reverse する。
> 2. 次の操作を **0 回以上**行う。
>   - 文字列の隣接する 2 文字を swap する。
> 
> 最小何回の swap 操作が必要であるか、計算せよ。

接頭辞とは文字列 $ Y $ が文字列 $ X $ の接頭辞であるとは、$ 1\ \leq\ |Y|\ \leq\ |X| $ であり、かつ $ X $ の最初の $ |Y| $ 文字が $ Y $ であることを指します。たとえば `ATC` は `ATCODER` の接頭辞ですが、`AGC` や `ATCODERGRANDCONTEST` は `ATCODER` の接頭辞ではありません。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $ $ K $ $ S $

## 输出格式

答えを $ K $ 行に出力してください。$ i $ 行目 $ (1\ \leq\ i\ \leq\ K) $ には $ k\ =\ i $ のときの答えを出力してください。

## 输入输出样例 #1

### 输入 #1

```
1 2
AC
```

### 输出 #1

```
0
0
```

## 输入输出样例 #2

### 输入 #2

```
5 1
CACAAACCCA
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
10 10
ACCCAAAACCCACCACAACA
```

### 输出 #3

```
1
2
3
3
3
3
3
3
3
3
```

## 输入输出样例 #4

### 输入 #4

```
50 10
ACCCCACAACAAAACCAACCCCACCAACACCAAAACACACAAAACCCCCACCAACACAACAACCCCAACAAACCCAACACACCCACACCAAACCCAAACA
```

### 输出 #4

```
10
17
20
22
23
24
25
26
26
26
```

## 输入输出样例 #5

### 输入 #5

```
72 10
CCCCACAAAAACCCACACCAAACCACCCCCAAAAACACCACCCCCAAAAAAACAAAAAACCCCCCACCCAAACAACACCACCACAAACCCAACCAACAACCCAAAACAACCCCACCACACACCACACCCACAAACACAACAACA
```

### 输出 #5

```
28
42
51
54
57
60
63
64
65
66
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1\,000\,000 $
- $ 1\ \leq\ K\ \leq\ 300\,000 $
- 文字列 $ S $ は $ N $ 個の `A` と $ N $ 個の `C` からなる $ 2N $ 文字の文字列である
- $ N $ と $ K $ は整数

### Sample Explanation 1

$ k\ =\ 1 $ のとき、最初黒板に書かれた文字列は `AC` となります。 $ k\ =\ 2 $ のとき、最初黒板に書かれた文字列は `ACAC` となります。 両方とも最初から AGC 語であるため、たとえば $ (l,\ r)\ =\ (1,\ 1) $ とすると、$ 0 $ 回の swap 操作を達成することができます。

### Sample Explanation 2

$ k\ =\ 1 $ のとき、黒板に書かれる文字列は `CACAAACCCA` となります。以下の手順で操作を行うと、swap 操作を $ 1 $ 回しか行う必要がありません。 1. $ (l,\ r)\ =\ (1,\ 4) $ を選択し、文字列の $ 1 $ から $ 4 $ 文字目を reverse する。文字列は `ACACAACCCA` となる。 2. 文字列の $ 9 $ 文字目と $ 10 $ 文字目を swap する。文字列は `ACACAACCAC` となり、これは AGC 語である。