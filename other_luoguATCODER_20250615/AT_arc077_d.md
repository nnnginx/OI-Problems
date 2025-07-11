# AT_arc077_d [ARC077F] SS

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc077/tasks/arc077_d

同じ文字列を $ 2 $ つ並べてできる文字列のことを偶文字列と呼ぶことにします。 例えば、 `xyzxyz` や `aaaaaa` は偶文字列ですが、`ababab` や `xyzxy` は偶文字列ではありません。

空でない文字列 $ S $ に対して、$ f(S) $ を 「$ S $ の後ろに $ 1 $ 文字以上の文字を追加してできる偶文字列のうち 最短の文字列」として定義します。 例えば、 $ f( $`abaaba`$ )= $`abaababaab` です。 このような文字列は空でない文字列に対してはちょうど $ 1 $ 通りに定まることが証明できます。

アルファベットの小文字からなる偶文字列 $ S $ が与えられます。 $ f^{10^{100}}\ (S) $ の $ l $ 文字目から $ r $ 文字目までに アルファベットの小文字がそれぞれ何回出現するかを求めて下さい。

$ f^{10^{100}}\ (S) $ というのは、 $ f(f(f(\ ...\ f(S)\ ...\ ))) $ のように、$ S $ を $ 10^{100} $ 回 $ f $ で写した文字列のことを指します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ l $ $ r $

## 输出格式

$ 26 $ 個の整数を空白区切りで $ 1 $ 行に出力せよ。 $ i $ 番目には、 $ f^{10^{100}}(S) $ の $ l $ 文字目から $ r $ 文字目までに $ i $ 番目の アルファベットが何回出現するかを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
abaaba
6 10
```

### 输出 #1

```
3 2 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

## 输入输出样例 #2

### 输入 #2

```
xx
1 1000000000000000000
```

### 输出 #2

```
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1000000000000000000 0 0
```

## 输入输出样例 #3

### 输入 #3

```
vgxgpuamkvgxgvgxgpuamkvgxg
1 1000000000000000000
```

### 输出 #3

```
87167725689669676 0 0 0 0 0 282080685775825810 0 0 0 87167725689669676 0 87167725689669676 0 0 87167725689669676 0 0 0 0 87167725689669676 141040342887912905 0 141040342887912905 0 0
```

## 说明/提示

### 制約

- $ 2\ \leq\ |S|\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ l\ \leq\ r\ \leq\ 10^{18} $
- $ S $ は小文字のアルファベットのみからなる偶文字列である。
- $ l,r $ は整数である。

### Sample Explanation 1

$ f( $`abaaba`$ )= $`abaababaab` なので、$ f^{10^{100}}(S) $ の最初の $ 10 $ 文字を取り出したものも やはり `abaababaab` となっています。よって、$ 6 $ 文字目から $ 10 $ 文字目は `abaab` です。 `abaab` には `a` が $ 3 $ 回、 `b` が $ 2 $ 回使われていて、 `c` から `z` までは $ 1 $ 回も出てこないので、 出力するべき値は $ 1 $ 番目が $ 3 $ で、 $ 2 $ 番目が $ 2 $ で、それ以外の $ 24 $ 個が $ 0 $ となります。