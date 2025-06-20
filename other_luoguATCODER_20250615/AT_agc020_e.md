# AT_agc020_e [AGC020E] Encoding Subsets

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc020/tasks/agc020_e

次のような、`0` と `1` からなる文字列をエンコードする規則を考えます。

- 文字列 `0`、`1` はそれぞれ `0`、`1` とエンコードできる。
- 文字列 $ A $、$ B $ をそれぞれ $ P $、$ Q $ とエンコードできる場合、文字列 $ AB $ を $ PQ $ とエンコードできる。
- 文字列 $ A $ を $ P $ とエンコードできる場合、$ K\ \geq\ 2 $ を正の整数として、文字列 $ AA...A $（$ A $ を $ K $ 個連結したもの）を `(`$ P $`x`$ K $`)` とエンコードできる。

例えば、文字列 `001001001` は `001001001`、`00(1(0x2)x2)1`、`(001x3)` などとエンコードすることができ、この他のエンコード方法も存在します。

また、次の条件が満たされるとき、文字列 $ A $ は文字列 $ B $ の *サブセット* であると呼びます。

- $ A $ と $ B $ は長さが等しく、どちらも `0` と `1` からなる。
- $ A_i $ = `1` であるようなすべての添字 $ i $ に対して、$ B_i $ = `1` でもある。

`0` と `1` からなる文字列 $ S $ が与えられます。$ S $ のすべてのサブセットについて、それぞれをエンコードする方法が何通り存在するか求め、それらの個数の総和を $ 998244353 $ で割ったあまりを求めてください。

## 输入格式

入力は標準入力から以下の形式で与えられる。

> $ S $

## 输出格式

$ S $ のすべてのサブセットについてのエンコード方法の個数の総和を $ 998244353 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
011
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
0000
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
101110
```

### 输出 #3

```
156
```

## 输入输出样例 #4

### 输入 #4

```
001110111010110001100000100111
```

### 输出 #4

```
363383189
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 100 $
- $ S $ は `0` と `1` からなる。

### Sample Explanation 1

$ S $ のサブセットは $ 4 $ 個存在し、 - `011` は `011`、`0(1x2)` とエンコードできます。 - `010` は `010` とエンコードできます。 - `001` は `001`、`(0x2)1` とエンコードできます。 - `000` は `000`、`0(0x2)`、`(0x2)0`、`(0x3)` とエンコードできます。 したがって、$ S $ のすべてのサブセットについてのエンコード方法の個数の総和は $ 2\ +\ 1\ +\ 2\ +\ 4\ =\ 9 $ 通りです。

### Sample Explanation 2

今回は $ S $ のサブセットは $ 1 $ 個しか存在しませんが、$ 10 $ 通りの方法でエンコードできます。

### Sample Explanation 4

結果を $ 998244353 $ で割ったあまりを出力することを忘れずに。