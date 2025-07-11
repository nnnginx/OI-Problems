# AT_abc357_e [ABC357E] Reachability in Functional Graph

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc357/tasks/abc357_e

頂点に $ 1 $ から $ N $ の番号がついた $ N $ 頂点 $ N $ 辺の有向グラフがあります。  
 全ての頂点の出次数は $ 1 $ で、頂点 $ i $ から出ている辺は頂点 $ a_i $ へ伸びています。  
 頂点の組 $ (u,\ v) $ であって、頂点 $ u $ から頂点 $ v $ へ到達可能であるものの個数を求めてください。

ここで、頂点 $ u $ から頂点 $ v $ へ到達可能であるとは、ある長さ $ K+1 $ の頂点の列 $ w_0,\ w_1,\ \dots,\ w_K $ であって次の条件を全て満たすものが存在することをいいます。特に、$ u\ =\ v $ の時は常に到達可能です。

- $ w_0\ =\ u $
- $ w_K\ =\ v $
- $ 0\ \leq\ i\ \lt\ K $ を満たす全ての $ i $ について、頂点 $ w_i $ から頂点 $ w_{i+1} $ へ伸びる辺が存在する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ \dots $ $ a_N $

## 输出格式

頂点の組 $ (u,\ v) $ であって、頂点 $ u $ から頂点 $ v $ へ到達可能であるものの個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
2 1 1 4
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
5
2 4 3 1 2
```

### 输出 #2

```
14
```

## 输入输出样例 #3

### 输入 #3

```
10
6 10 4 1 5 9 8 6 5 1
```

### 输出 #3

```
41
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ a_i\ \leq\ N $
- 入力される値は全て整数
 
### Sample Explanation 1

頂点 $ 1 $ から到達可能である頂点は頂点 $ 1,\ 2 $ です。 頂点 $ 2 $ から到達可能である頂点は頂点 $ 1,\ 2 $ です。 頂点 $ 3 $ から到達可能である頂点は頂点 $ 1,\ 2,\ 3 $ です。 頂点 $ 4 $ から到達可能である頂点は頂点 $ 4 $ のみです。 よって、頂点の組 $ (u,\ v) $ であって頂点 $ u $ から頂点 $ v $ へ到達可能であるものの個数は $ 8 $ 個です。 頂点 $ 4 $ から出ている辺は自己ループ、すなわち頂点 $ 4 $ 自身へ伸びている辺である点に注意してください。