# AT_abc180_f [ABC180F] Unbranched

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc180/tasks/abc180_f

頂点にラベルが付き辺にはラベルが付いていない $ N $ 頂点 $ M $ 辺の単純とも連結とも限らないグラフであって、以下の条件を満たすものの個数を $ 10^9+7 $ で割ったあまりを求めてください。

- 自己ループを持たない
- すべての頂点の次数が $ 2 $ 以下である
- 各連結成分のサイズを並べたとき、その最大値がちょうど $ L $ である

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ L $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2 3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4 3 2
```

### 输出 #2

```
6
```

## 输入输出样例 #3

### 输入 #3

```
300 290 140
```

### 输出 #3

```
211917445
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 300 $
- $ 1\leq\ M\ \leq\ N $
- $ 1\ \leq\ L\ \leq\ N $
- 入力はすべて整数

### Sample Explanation 1

頂点に $ 1 $ から $ N $ の番号を付けたとき、以下の $ 3 $ 通りのグラフが条件を満たします。 - $ 1-2 $ 間と $ 2-3 $ 間に辺がある。 - $ 1-2 $ 間と $ 1-3 $ 間に辺がある。 - $ 1-3 $ 間と $ 2-3 $ 間に辺がある。