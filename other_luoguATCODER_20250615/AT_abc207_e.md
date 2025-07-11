# AT_abc207_e [ABC207E] Mod i

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc207/tasks/abc207_e

長さ $ N $ の数列 $ A $ が与えられます。$ A $ をいくつかの連続した空でない部分列 $ B_1,B_2,\ldots,B_k $ に切り分ける方法であって、以下の条件を満たすものの個数を求めてください。

- 全ての $ i\ (1\ \leq\ i\ \leq\ k) $ について、$ B_i $ に含まれる要素の総和が $ i $ で割り切れる。

答えは非常に大きくなることがあるので、$ (10^9+7) $ で割ったあまりを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

問題文中の条件を満たすような切り分け方の個数を $ (10^9+7) $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 2 3 4
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5
8 6 3 3 3
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
10
791754273866483 706434917156797 714489398264550 918142301070506 559125109706263 694445720452148 648739025948445 869006293795825 718343486637033 934236559762733
```

### 输出 #3

```
15
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 3000 $
- $ 1\ \leq\ A_i\ \leq\ 10^{15} $
- 入力は全て整数

### Sample Explanation 1

以下の $ 3 $ 通りの切り分け方があります。 - $ (1),(2),(3),(4) $ - $ (1,2,3),(4) $ - $ (1,2,3,4) $

### Sample Explanation 3

入力が $ 32 $ bit 整数型に収まりきらない場合があります。