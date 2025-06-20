# AT_dp_v Subtree

## 题目描述

[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_v

$ N $ 頂点の木があります。 頂点には $ 1,\ 2,\ \ldots,\ N $ と番号が振られています。 各 $ i $ ($ 1\ \leq\ i\ \leq\ N\ -\ 1 $) について、$ i $ 番目の辺は頂点 $ x_i $ と $ y_i $ を結んでいます。

太郎君は、各頂点を白または黒で塗ることにしました。 このとき、どの黒い頂点からどの黒い頂点へも、黒い頂点のみを辿って到達できるようにします。

正整数 $ M $ が与えられます。 各 $ v $ ($ 1\ \leq\ v\ \leq\ N $) について、次の質問に答えてください。

- 頂点 $ v $ が黒であるような頂点の色の組合せは何通りか？ $ M $ で割った余りを求めよ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ $ : $ $ x_{N\ -\ 1} $ $ y_{N\ -\ 1} $

## 输出格式

$ N $ 行出力せよ。 $ v $ ($ 1\ \leq\ v\ \leq\ N $) 行目には、次の質問に対する答えを出力せよ。

- 頂点 $ v $ が黒であるような頂点の色の組合せは何通りか？ $ M $ で割った余りを求めよ。

## 输入输出样例 #1

### 输入 #1

```
3 100
1 2
2 3
```

### 输出 #1

```
3
4
3
```

## 输入输出样例 #2

### 输入 #2

```
4 100
1 2
1 3
1 4
```

### 输出 #2

```
8
5
5
5
```

## 输入输出样例 #3

### 输入 #3

```
1 100
```

### 输出 #3

```
1
```

## 输入输出样例 #4

### 输入 #4

```
10 2
8 5
10 8
6 5
1 5
4 8
2 10
3 6
9 2
1 7
```

### 输出 #4

```
0
0
1
1
1
0
1
0
1
1
```

## 说明/提示

### 制約

- 入力はすべて整数である。
- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 2\ \leq\ M\ \leq\ 10^9 $
- $ 1\ \leq\ x_i,\ y_i\ \leq\ N $
- 与えられるグラフは木である。

### Sample Explanation 1

頂点の色の組合せは次図の $ 7 $ 通りです。 このうち、頂点 $ 1 $ が黒であるようなものは $ 3 $ 通り、頂点 $ 2 $ が黒であるようなものは $ 4 $ 通り、頂点 $ 3 $ が黒であるようなものは $ 3 $ 通りです。 !\[\](https://img.atcoder.jp/dp/subtree\_0\_muffet.png)

### Sample Explanation 4

答えを $ M $ で割った余りを出力することを忘れずに。