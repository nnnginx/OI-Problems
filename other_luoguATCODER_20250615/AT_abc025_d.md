# AT_abc025_d [ABC025D] 25個の整数

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc025/tasks/abc025_d

高橋君は縦 $ 5 $ マス、横 $ 5 $ マスの盤面に $ 1 $ から $ 25 $ までの整数を $ 1 $ つずつ書き込もうとしています。

高橋君は以下の条件をすべて満たすように整数を配置しようと考えています。

- 整数は各マスに $ 1 $ つずつ割り当てる。
- 縦または横に連続する $ 3 $ つの整数をどのように取り出しても、それらは昇順または降順になっていない。すなわち、上から $ i\ (1\ ≦\ i\ ≦\ 5) $ 番目、左から $ j\ (1\ ≦\ j\ ≦\ 5) $ 番目のマスに書かれた整数を $ n_{i,j} $ としたとき、以下の $ 2 $ 条件が成立する。
- $ n_{i,j}\ ＜\ n_{i+1,j}\ ＜\ n_{i+2,j} $ あるいは $ n_{i,j}\ ＞\ n_{i+1,j}\ ＞\ n_{i+2,j} $ を満たす整数組 $ (i,j)\ (1\ ≦\ i\ ≦\ 3,\ 1\ ≦\ j\ ≦\ 5) $ が存在しない。
- $ n_{i,j}\ ＜\ n_{i,j+1}\ ＜\ n_{i,j+2} $ あるいは $ n_{i,j}\ ＞\ n_{i,j+1}\ ＞\ n_{i,j+2} $ を満たす整数組 $ (i,j)\ (1\ ≦\ i\ ≦\ 5,\ 1\ ≦\ j\ ≦\ 3) $ が存在しない。


すでにいくつかのマスについては、どの整数を書き込むかは決まっています。あなたの課題は、上記の条件を満たすような残りの整数の配置の総数を計算することです。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ x_{1,1} $ $ x_{1,2} $ $ x_{1,3} $ $ x_{1,4} $ $ x_{1,5} $ $ x_{2,1} $ $ x_{2,2} $ $ x_{2,3} $ $ x_{2,4} $ $ x_{2,5} $ $ x_{3,1} $ $ x_{3,2} $ $ x_{3,3} $ $ x_{3,4} $ $ x_{3,5} $ $ x_{4,1} $ $ x_{4,2} $ $ x_{4,3} $ $ x_{4,4} $ $ x_{4,5} $ $ x_{5,1} $ $ x_{5,2} $ $ x_{5,3} $ $ x_{5,4} $ $ x_{5,5} $

- $ 1 $ 行目には、$ 5 $ つの整数 $ x_{1,1}\ (0\ ≦\ x_{1,1}\ ≦\ 25) $ と $ x_{1,2}\ (0\ ≦\ x_{1,2}\ ≦\ 25) $ と $ x_{1,3}\ (0\ ≦\ x_{1,3}\ ≦\ 25) $ と $ x_{1,4}\ (0\ ≦\ x_{1,4}\ ≦\ 25) $ と $ x_{1,5}\ (0\ ≦\ x_{1,5}\ ≦\ 25) $ が空白区切りで書かれている。
- $ 2 $ 行目には、$ 5 $ つの整数 $ x_{2,1}\ (0\ ≦\ x_{2,1}\ ≦\ 25) $ と $ x_{2,2}\ (0\ ≦\ x_{2,2}\ ≦\ 25) $ と $ x_{2,3}\ (0\ ≦\ x_{2,3}\ ≦\ 25) $ と $ x_{2,4}\ (0\ ≦\ x_{2,4}\ ≦\ 25) $ と $ x_{2,5}\ (0\ ≦\ x_{2,5}\ ≦\ 25) $ が空白区切りで書かれている。
- $ 3 $ 行目には、$ 5 $ つの整数 $ x_{3,1}\ (0\ ≦\ x_{3,1}\ ≦\ 25) $ と $ x_{3,2}\ (0\ ≦\ x_{3,2}\ ≦\ 25) $ と $ x_{3,3}\ (0\ ≦\ x_{3,3}\ ≦\ 25) $ と $ x_{3,4}\ (0\ ≦\ x_{3,4}\ ≦\ 25) $ と $ x_{3,5}\ (0\ ≦\ x_{3,5}\ ≦\ 25) $ が空白区切りで書かれている。
- $ 4 $ 行目には、$ 5 $ つの整数 $ x_{4,1}\ (0\ ≦\ x_{4,1}\ ≦\ 25) $ と $ x_{4,2}\ (0\ ≦\ x_{4,2}\ ≦\ 25) $ と $ x_{4,3}\ (0\ ≦\ x_{4,3}\ ≦\ 25) $ と $ x_{4,4}\ (0\ ≦\ x_{4,4}\ ≦\ 25) $ と $ x_{4,5}\ (0\ ≦\ x_{4,5}\ ≦\ 25) $ が空白区切りで書かれている。
- $ 5 $ 行目には、$ 5 $ つの整数 $ x_{5,1}\ (0\ ≦\ x_{5,1}\ ≦\ 25) $ と $ x_{5,2}\ (0\ ≦\ x_{5,2}\ ≦\ 25) $ と $ x_{5,3}\ (0\ ≦\ x_{5,3}\ ≦\ 25) $ と $ x_{5,4}\ (0\ ≦\ x_{5,4}\ ≦\ 25) $ と $ x_{5,5}\ (0\ ≦\ x_{5,5}\ ≦\ 25) $ が空白区切りで書かれている。
 
 上記 $ 25 $ 個の整数は、以下の情報を表している。 - 整数 $ x_{i,j}\ (1\ ≦\ i\ ≦\ 5,\ 1\ ≦\ j\ ≦\ 5) $ は上から $ i $ 番目、左から $ j $ 番目のマスに書かれる整数に関する情報である。$ x_{i,j}\ =\ 0 $ ならそのマスに書かれる整数が決まっていないことを、$ x_{i,j}\ ≠\ 0 $ ならそのマスに書かれる整数が $ x_{i,j} $ であることを表す。
 
 また、入力は以下の条件を満たす。 - $ 1 $ 以上 $ 5 $ 以下の $ 4 $ つの整数組 $ i,j,k,l $ に関して、$ x_{i,j}\ ≧\ 1 $ かつ $ x_{k,l}\ ≧\ 1 $ かつ $ (i,j)\ ≠\ (k,l) $ ならば、$ x_{i,j}\ ≠\ x_{k,l} $。
- $ x_{i,j}\ ≠\ 0 $ を満たす整数組 $ (i,j)\ (1\ ≦\ i\ ≦\ 5,\ 1\ ≦\ j\ ≦\ 5) $ は $ 5 $ 個以上存在する。

## 输出格式

条件を満たすような残りの整数の配置の総数を $ 1000000007\ (=\ 1,000,000,007) $ で割った余りを $ 1 $ 行に出力せよ。出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
0 0 15 2 7
0 0 16 1 22
20 25 4 19 0
3 23 9 18 10
17 0 5 21 8
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
10 14 13 15 11
16 0 17 0 18
0 19 0 20 9
21 12 22 0 23
0 24 0 25 0
```

### 输出 #2

```
40320
```

## 输入输出样例 #3

### 输入 #3

```
1 2 3 4 5
6 7 8 9 10
11 12 13 14 15
16 17 18 19 20
0 0 0 0 0
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
1 25 2 24 3
23 4 22 5 21
6 20 7 19 8
18 9 17 10 16
11 15 12 14 13
```

### 输出 #4

```
1
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- データセット $ 1 $ において、すべての入力には、$ x_{i,j}\ ≠\ 0 $ を満たす整数組 $ (i,j)\ (1\ ≦\ i\ ≦\ 5,\ 1\ ≦\ j\ ≦\ 5) $ が $ 17 $ 個以上存在する。データセット $ 1 $ に正解した場合は、$ 30 $ 点が与えられる。
- 追加制約のないデータセット $ 2 $ に正解した場合は、上記とは別に $ 70 $ 点が与えられる。

### Sample Explanation 1

\- まだ書かれていない整数は $ 6,\ 11,\ 12,\ 13,\ 14,\ 24 $ の $ 6 $ つです。以下の $ 2 $ 通りが、条件を満たす配置です。 14121527131116122202541963239181017245218 14131527121116122202541963239181017245218

### Sample Explanation 2

\- どのように残りを書いても条件を満たします。

### Sample Explanation 3

\- どのように置いても条件を満たさない場合があります。

### Sample Explanation 4

\- すでにすべての整数の配置が決まっている場合もあります。