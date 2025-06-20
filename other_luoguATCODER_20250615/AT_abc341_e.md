# AT_abc341_e [ABC341E] Alternating String

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc341/tasks/abc341_e

`0` と `1` のみからなる文字列であって、文字列中のどの連続する $ 2 $ 文字も異なるようなものを **良い文字列** とよびます。  
`0` と `1` のみからなる長さ $ N $ の文字列 $ S $ が与えられます。 $ Q $ 個のクエリが与えられるので、順に処理してください。  
クエリは次の $ 2 $ 種類です。

- `1 L R` : $ S $ の $ L $ 文字目から $ R $ 文字目までの `0` と `1` を反転させる。すなわち、$ L\leq\ i\leq\ R $ をみたす整数 $ i $ について、$ S $ の $ i $ 文字目が `0` ならば `1` に、`1` ならば `0` に変更する。
- `2 L R` : $ S $ の $ L $ 文字目から $ R $ 文字目までを（順番を変えずに）抜き出した長さ $ (R-L+1) $ の文字列を $ S' $ とする。$ S' $ が良い文字列ならば `Yes` を、そうでないならば `No` を出力する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ Q $ $ S $ $ query_1 $ $ query_2 $ $ \vdots $ $ query_Q $

各クエリ $ query_i $ $ (1\leq\ i\leq\ Q) $ は、

> $ 1 $ $ L $ $ R $

または、

> $ 2 $ $ L $ $ R $

の形で与えられる。

## 输出格式

$ 2 $ 種類目のクエリの数を $ K $ 個として、$ K $ 行出力せよ。  
$ i $ 行目には $ i $ 個目の $ 2 $ 種類目のクエリに対する出力を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 6
10100
2 1 3
2 1 5
1 1 4
2 1 5
1 3 3
2 2 4
```

### 输出 #1

```
Yes
No
Yes
No
```

## 输入输出样例 #2

### 输入 #2

```
1 2
1
1 1 1
2 1 1
```

### 输出 #2

```
Yes
```

## 说明/提示

### 制約

- $ 1\leq\ N,\ Q\leq\ 5\times\ 10^5 $
- $ S $ は `0` と `1` のみからなる長さ $ N $ の文字列
- $ 1,2 $ 種類目のクエリについて、$ 1\leq\ L\leq\ R\leq\ N $
- $ 2 $ 種類目のクエリが少なくとも $ 1 $ つ存在する。
- $ N $, $ Q $, $ L $, $ R $ は整数

### Sample Explanation 1

最初、$ S= $`10100` です。このとき、クエリを与えられた順に処理すると以下のようになります。 - $ 1 $ 番目のクエリについて、$ S $ の $ 1 $ 文字目から $ 3 $ 文字目までを抜き出した文字列は $ S'= $`101` です。これは良い文字列なので `Yes` を出力します。 - $ 2 $ 番目のクエリについて、$ S $ の $ 1 $ 文字目から $ 5 $ 文字目までを抜き出した文字列は $ S'= $`10100` です。これは良い文字列でないので `No` を出力します。 - $ 3 $ 番目のクエリについて、$ S $ の $ 1 $ 文字目から $ 4 $ 文字目までの `0` と `1` を反転させます。文字列 $ S $ は $ S= $`01010` となります。 - $ 4 $ 番目のクエリについて、$ S $ の $ 1 $ 文字目から $ 5 $ 文字目までを抜き出した文字列は $ S'= $`01010` です。これは良い文字列なので `Yes` を出力します。 - $ 5 $ 番目のクエリについて、$ S $ の $ 3 $ 文字目の `0` と `1` を反転させます。文字列 $ S $ は $ S= $`01110` となります。 - $ 6 $ 番目のクエリについて、$ S $ の $ 2 $ 文字目から $ 4 $ 文字目までを抜き出した文字列は $ S'= $`111` です。これは良い文字列でないので `No` を出力します。

### Sample Explanation 2

`0` または `1` の $ 1 $ 文字からなる文字列は良い文字列の条件をみたすことに注意してください。