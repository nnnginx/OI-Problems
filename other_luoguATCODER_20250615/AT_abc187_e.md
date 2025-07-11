# AT_abc187_e [ABC187E] Through Path

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc187/tasks/abc187_e

$ N $ 頂点 $ N-1 $ 辺から成る木があり、頂点には $ 1,\ 2,\ \dots,\ N $ の番号が、辺には $ 1,\ 2,\ \dots,\ N-1 $ の番号がついています。辺 $ i $ は頂点 $ a_i $ と頂点 $ b_i $ を結びます。 この木の各頂点には $ 1 $ つの整数が書かれています。頂点 $ i $ に書かれている整数を $ c_i $ とします。はじめ、 $ c_i\ =\ 0 $ です。

$ Q $ 個のクエリが与えられます。 $ i $ 番目のクエリでは、整数 $ t_i,\ e_i,\ x_i $ が与えられます。クエリの内容は以下の通りです。

- $ t_i\ =\ 1 $ のとき : 頂点 $ a_{e_i} $ から辺をたどって頂点 $ b_{e_i} $ を通らずに到達できるような全ての頂点 $ v $ に対して、$ c_v $ を $ c_v\ +\ x_i $ に書き換える。
- $ t_i\ =\ 2 $ のとき : 頂点 $ b_{e_i} $ から辺をたどって頂点 $ a_{e_i} $ を通らずに到達できるような全ての頂点 $ v $ に対して、$ c_v $ を $ c_v\ +\ x_i $ に書き換える。

すべてのクエリを処理した後、各頂点に書かれた整数を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ b_1 $ $ \vdots $ $ a_{N-1} $ $ b_{N-1} $ $ Q $ $ t_1 $ $ e_1 $ $ x_1 $ $ \vdots $ $ t_Q $ $ e_Q $ $ x_Q $

## 输出格式

すべてのクエリを処理した後の $ c_1,\ c_2,\ \dots,\ c_N $ をこの順に改行区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
1 2
2 3
2 4
4 5
4
1 1 1
1 4 10
2 1 100
2 2 1000
```

### 输出 #1

```
11
110
1110
110
100
```

## 输入输出样例 #2

### 输入 #2

```
7
2 1
2 3
4 2
4 5
6 1
3 7
7
2 2 1
1 3 2
2 2 4
1 6 8
1 3 16
2 4 32
2 1 64
```

### 输出 #2

```
72
8
13
26
58
72
5
```

## 输入输出样例 #3

### 输入 #3

```
11
2 1
1 3
3 4
5 2
1 6
1 7
5 8
3 9
3 10
11 4
10
2 6 688
1 10 856
1 8 680
1 8 182
2 2 452
2 4 183
2 6 518
1 3 612
2 6 339
2 3 206
```

### 输出 #3

```
1657
1657
2109
1703
1474
1657
3202
1474
1247
2109
2559
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ a_i,\ b_i\ \le\ N $
- 与えられるグラフは木である
- $ 1\ \le\ Q\ \le\ 2\ \times\ 10^5 $
- $ t_i\ \in\ \{1,\ 2\} $
- $ 1\ \le\ e_i\ \le\ N-1 $
- $ 1\ \le\ x_i\ \le\ 10^9 $

### Sample Explanation 1

$ 1 $ 番目のクエリでは、頂点 $ 1 $ から始めて頂点 $ 2 $ を通らずに到達できる頂点 $ 1 $ に $ 1 $ を足します。 $ 2 $ 番目のクエリでは、頂点 $ 4 $ から始めて頂点 $ 5 $ を通らずに到達できる頂点 $ 1,\ 2,\ 3,\ 4 $ に $ 10 $ を足します。 $ 3 $ 番目のクエリでは、頂点 $ 2 $ から始めて頂点 $ 1 $ を通らずに到達できる頂点 $ 2,\ 3,\ 4,\ 5 $ に $ 100 $ を足します。 $ 4 $ 番目のクエリでは、頂点 $ 3 $ から始めて頂点 $ 2 $ を通らずに到達できる頂点 $ 3 $ に $ 1000 $ を足します。