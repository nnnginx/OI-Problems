# AT_joi2020_yo1c_b キャピタリゼーション (Capitalization)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2020yo1c/tasks/joi2020_yo1c_b

JOI 君は長さ $ N $ の文字列 $ S $ を見つけた．$ S $ に含まれる文字はすべて英小文字である．

JOI 君はこの文字列から自分の名前である `joi` が連続している部分を先頭から順にすべて探しだすことにした．そして `joi` を見つけるたびに，強調のためにそれを大文字の `JOI` に置き換えることにした．

文字列 $ S $ が与えられたとき，$ S $ に含まれる `joi` をすべて `JOI` に置き換えた文字列を出力するプログラムを作成せよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $

## 输出格式

$ S $ に含まれる `joi` をすべて `JOI` に置き換えた文字列を $ 1 $ 行で出力せよ．

## 输入输出样例 #1

### 输入 #1

```
11
joinojoijin
```

### 输出 #1

```
JOInoJOIjin
```

## 输入输出样例 #2

### 输入 #2

```
16
jjooiiijoiojioij
```

### 输出 #2

```
jjooiiiJOIojioij
```

## 输入输出样例 #3

### 输入 #3

```
13
nihongoutenai
```

### 输出 #3

```
nihongoutenai
```

## 说明/提示

### 制約

- $ 3\ \leqq\ N\ \leqq\ 100 $．
- $ S $ は長さ $ N $ の文字列である．
- $ S $ は英小文字からなる．

### Sample Explanation 1

$ 1 $ 文字目から $ 3 $ 文字目の `joi` と $ 6 $ 文字目から $ 8 $ 文字目までの `joi` を `JOI` に置き換える．

### Sample Explanation 3

$ S $ に `joi` がひとつも含まれない場合もあることに注意せよ．