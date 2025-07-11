# AT_ttpc2015_c おおおかやま

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ttpc2015/tasks/ttpc2015_c

okayama国の首都ookayamaでは、`ookayama`の先頭に$ 1 $個以上の任意の個数の`o`が付加された文字列のことを良い文字列と呼ぶ。

あなたの仕事は文字列$ S $を次のルールで処理するプログラムを書くことである。

- 手順$ 1 $. $ S $の部分文字列に良い文字列が存在するならば手順$ 2 $へ、存在しないならば処理を終了する。
- 手順$ 2 $. 良い文字列であるような$ S $の部分文字列のうち、長さが最長のものを選びこれを$ T $として手順$ 3 $へ。最長のものが複数ある場合は最も左側にあるものを選ぶ。
- 手順$ 3 $. $ T $に`oo`という部分文字列が存在するならば、そのうち最も左側にあるものを`O`へ置換して手順$ 4 $へ、存在しないならば手順$ 1 $へ。
- 手順$ 4 $. $ T $に`OO`という部分文字列が存在するならば、そのうち最も左側にあるものを`o`へ置換する。存在するかどうかにかかわらず手順$ 3 $へ。

処理終了後の$ S $を求めよ。この処理結果が何に用いられるかは機密情報であるため、あなたは知る必要はない。

ある文字列$ T $が$ S $の$ i\ (1\ \leq\ i\ \leq\ |S|) $文字目から$ j\ (i\ \leq\ j\ \leq\ |S|) $文字目までを取り出したものであるとき、$ T $は$ S $の部分文字列であると呼ぶ。ここで$ |\ S\ | $は文字列$ S $の長さを表す。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

$ 1 $ 行目に処理すべき文字列$ S(1\ \leq\ |\ S\ |\ \leq\ 100) $が与えられる。$ S $は英小文字のみからなることが保証される。

## 输出格式

処理終了後の$ S $を$ 1 $行に出力せよ。改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
ooookayama
```

### 输出 #1

```
okayama
```

## 输入输出样例 #2

### 输入 #2

```
ooookayamaoooookayama
```

### 输出 #2

```
okayamaOkayama
```

## 输入输出样例 #3

### 输入 #3

```
okayama
```

### 输出 #3

```
okayama
```

## 输入输出样例 #4

### 输入 #4

```
ookayama
```

### 输出 #4

```
ookayama
```

## 输入输出样例 #5

### 输入 #5

```
ooookayamakenooooookayamashiookayama
```

### 输出 #5

```
okayamakenOokayamashiookayama
```

## 说明/提示

### Sample Explanation 1

文字列`ooookayama`に対し、処理を行うと、以下のような順序で扱われる。 1. 手順$ 1 $において$ S $の部分文字列に良い文字列は存在する。 2. 手順$ 2 $において良い文字列であって$ S $の部分文字列であるようなもののうち長さが最長のものは$ 1 $番目の`o`から始まる部分文字列である、`ooookayama`である。これを$ T $とする。 3. 手順$ 3 $において$ T $に存在する`oo`という部分文字列のうち、最も左側にあるものを`O`に置換する。$ T $は`Oookayama`となる。 4. 手順$ 4 $において$ T $に`OO`という部分文字列は存在しない。 5. 手順$ 3 $において$ T $に存在する`oo`という部分文字列のうち、最も左側にあるものを`O`に置換する。$ T $は`OOkayama`となる。 6. 手順$ 4 $において$ T $に存在する`OO`という部分文字列のうち、最も左側にあるものを`o`に置換する。$ T $は`okayama`となる。 7. 手順$ 3 $において$ T $に`oo`という部分文字列は存在しない。 8. 手順$ 1 $において$ S $は`okayama`である。$ S $の部分文字列に良い文字列は存在しない。処理を終了する。

### Sample Explanation 2

$ S $の部分文字列には、良い文字列が複数存在することもある。最長のものかつ最も左側にあるものから処理する必要があることに注意せよ。また、与えられる入力には英大文字は含まれないものの、答えや処理の過程には現れる可能性があることに注意せよ。

### Sample Explanation 3

文字列`okayama`の部分文字列には良い文字列は存在しない。

### Sample Explanation 4

文字列`ookayama`の部分文字列には良い文字列は存在しない。良い文字列とは`ookayama`の先頭に$ 1 $個以上の任意の個数の`o`が付加された文字列のことであるため`ookayama`は条件を満たさない。