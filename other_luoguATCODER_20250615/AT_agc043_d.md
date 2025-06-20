# AT_agc043_d [AGC043D] Merge Triplets

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc043/tasks/agc043_d

正整数 $ N $ が与えられます。 $ (1,2,\cdots,3N) $ の順列 $ (P_1,P_2,\cdots,P_{3N}) $であって、次の操作によって生成されうるものの数を求めてください。 ただし、答えは非常に大きくなることがあるので、素数 $ M $ で割ったあまりを求めてください。

- 長さ $ 3 $ の数列を $ N $ 個用意する。この数列たちを $ A_1,A_2,\cdots\ ,A_N $ とする。この $ 3N $ 個の値には $ 1 $ から $ 3N $ がちょうど一度ずつ登場せねばならない。
- 空の数列 $ P $ を用意する。以下の操作を $ 3N $ 回繰り返す。
  - 各数列 $ A_i $ のうち、空でないものの先頭の要素を見て、そのうち最小の要素を $ x $ とする。
  - $ x $ を $ A_i $ から消去する。 $ P $ の最後尾に $ x $ を追加する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式

条件を満たす順列の数を $ M $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 998244353
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
2 998244353
```

### 输出 #2

```
261
```

## 输入输出样例 #3

### 输入 #3

```
314 1000000007
```

### 输出 #3

```
182908545
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2000 $
- $ 10^8\ \leq\ M\ \leq\ 10^9+7 $
- $ M $ は素数
- 入力はすべて整数

### Sample Explanation 1

すべての長さ $ 3 $ の順列が条件を満たします。