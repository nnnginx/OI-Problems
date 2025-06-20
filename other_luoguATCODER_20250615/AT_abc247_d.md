# AT_abc247_d [ABC247D] Cylinder

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc247/tasks/abc247_d

空の筒があります。$ Q $ 個のクエリが与えられるので順に処理してください。  
クエリは次の $ 2 $ 種類のいずれかです。

- `1 x c`：数 $ x $ が書かれたボールを筒の右側から $ c $ 個入れる
- `2 c`：筒の左側からボールを $ c $ 個取り出し、取り出したボールに書かれている数の合計を出力する

なお、筒の中でボールの順序が入れ替わることはないものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ Q $ $ {\rm\ query}_1 $ $ \vdots $ $ {\rm\ query}_Q $

$ i $ 番目のクエリを表す $ {\rm\ query}_i $ は以下の $ 2 $ 種類のいずれかである。

> $ 1 $ $ x $ $ c $

> $ 2 $ $ c $

## 输出格式

`2 c` のクエリに対する答えを順に改行区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 2 3
2 2
1 3 4
2 3
```

### 输出 #1

```
4
8
```

## 输入输出样例 #2

### 输入 #2

```
2
1 1000000000 1000000000
2 1000000000
```

### 输出 #2

```
1000000000000000000
```

## 输入输出样例 #3

### 输入 #3

```
5
1 1 1
1 1 1
1 1 1
1 1 1
1 1 1
```

### 输出 #3

```

```

## 说明/提示

### 制約

- $ 1\ \leq\ Q\ \leq\ 2\times\ 10^5 $
- $ 0\ \leq\ x\ \leq\ 10^9 $
- $ 1\ \leq\ c\ \leq\ 10^9 $
- `2 c` のクエリが与えられるとき、筒の中には $ c $ 個以上のボールがある
- 入力に含まれる値は全て整数である

### Sample Explanation 1

\- $ 1 $ 番目のクエリでは、$ 2 $ が書かれたボールを筒の右側から $ 3 $ 個入れます。 筒の中のボールに書かれた数は左から順に $ (2,2,2) $ となります。 - $ 2 $ 番目のクエリでは、筒の左側からボールを $ 2 $ 個取り出します。 取り出されたボールに書かれている数はそれぞれ $ 2,2 $ であり、合計は $ 4 $ であるため、これを出力します。 筒の中のボールに書かれた数は左から順に $ (2) $ となります。 - $ 3 $ 番目のクエリでは、$ 3 $ が書かれたボールを筒の右側から $ 4 $ 個入れます。 筒の中のボールに書かれた数は左から順に $ (2,3,3,3,3) $ となります。 - $ 4 $ 番目のクエリでは、筒の左側からボールを $ 3 $ 個取り出します。 取り出されたボールに書かれている数はそれぞれ $ 2,3,3 $ であり、合計は $ 8 $ であるため、これを出力します。 筒の中のボールに書かれた数は左から順に $ (3,3) $ となります。

### Sample Explanation 3

出力するものがないこともあります。