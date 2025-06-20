# AT_abc214_h [ABC214H] Collecting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc214/tasks/abc214_h

$ N $ 頂点 $ M $ 辺の有向グラフがあります。  
 頂点は $ 1,\ \dots,\ N $ と番号付けられており、$ i\ \,\ (1\ \leq\ i\ \leq\ M) $ 番目の辺は頂点 $ A_i $ から頂点 $ B_i $ に向けて張られています。

はじめ、頂点 $ i\ \,\ (\ 1\ \leq\ i\ \leq\ N) $ には $ X_i $ 個の落とし物があります。これらの落とし物を $ K $ 人で拾うことになりました。

$ K $ 人は $ 1 $ 人ずつグラフ上を移動します。各々は次のような行動をとります。

- 頂点 $ 1 $ から出発し、辺をたどって移動することを任意の有限回繰り返す。訪れた各頂点（頂点 $ 1 $ も含む）について、落とし物がまだ拾われていなければ、全て拾う。

合計で最大何個の落とし物を拾うことができるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_M $ $ B_M $ $ X_1 $ $ \ldots $ $ X_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 5 2
1 2
2 3
3 2
1 4
1 5
1 4 5 2 8
```

### 输出 #1

```
18
```

## 输入输出样例 #2

### 输入 #2

```
3 1 10
2 3
1 100 100
```

### 输出 #2

```
1
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ K\ \leq\ 10 $
- $ 1\ \leq\ A_i,\ B_i\ \leq\ N $
- $ A_i\ \neq\ B_i $
- $ i\ \neq\ j $ ならば、$ A_i\ \neq\ A_j $ または $ B_i\ \neq\ B_j $
- $ 1\ \leq\ X_i\ \leq\ 10^9 $
- 入力は全て整数である。

### Sample Explanation 1

$ 2 $ 人がそれぞれ次のように行動することで、$ 18 $ 個の落とし物を拾うことができます。 - $ 1 $ 人目は、頂点 $ 1\ \rightarrow\ 2\ \rightarrow\ 3\ \rightarrow\ 2 $ の順に移動し、頂点 $ 1,\ 2,\ 3 $ にある落とし物を拾う。 - $ 2 $ 人目は、頂点 $ 1\ \rightarrow\ 5 $ の順に移動し、頂点 $ 5 $ にある落とし物を拾う。 $ 19 $ 個以上の落とし物を拾うことはできないので、$ 18 $ を出力します。