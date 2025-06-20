# AT_nikkei2019_final_e Erasure

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-final/tasks/nikkei2019_final_e

$ 1 $ から $ N $ までの番号のついた $ N $ 個のブロックがあります。 また、整数 $ K $ が与えられます。

魔法使いのコウさんは、魔法を唱えてこれらのブロックを消し去ろうとしています。 彼は、以下のような魔法を唱えることができます。

- $ 1\ \leq\ l\ \leq\ r\ \leq\ N $, $ r-l\ \geq\ K $ を満たす整数の組 $ (l,r) $ を選び、 番号が $ l $ 以上 $ r $ 以下の（まだ消されていない）ブロックをすべて消す。

つまり、彼が唱えられる魔法は $ (l,rの選び方の総数)\ =(N-K)\ \times\ (N-K+1)\ /\ 2 $ 種類あります。

それぞれの魔法を唱えるか唱えないかの組み合わせは全部で $ 2^{(N-K)\ \times\ (N-K+1)\ /\ 2} $ 通りあります。 コウさんは、このうち最終的にブロックをすべて消し去ることのできる組み合わせが何通りあるかに興味を持っています。

コウさんのために、最終的にブロックをすべて消し去ることのできる組み合わせが何通りあるかを求めてください。 ただし、答えは非常に大きくなることがあるので、答えを $ 10^9+7 $ で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式

最終的にブロックをすべて消し去ることのできる組み合わせの個数を $ 10^9+7 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 1
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
10 5
```

### 输出 #2

```
30784
```

## 输入输出样例 #3

### 输入 #3

```
5000 250
```

### 输出 #3

```
844653816
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 5000 $
- $ 0\ \leq\ K\ \leq\ N-1 $
- 入力される値はすべて整数である。

### Sample Explanation 1

コウさんが唱えられる魔法は、$ (l,r)=(1,2),(2,3),(1,3) $ の $ 3 $ 種類です。 最終的にブロックをすべて消し去ることのできる組み合わせは、以下の $ 5 $ 通りです。 - $ (1,2) $ と $ (2,3) $ - $ (1,2) $ と $ (1,3) $ - $ (1,2) $ と $ (2,3) $ と $ (1,3) $ - $ (2,3) $ と $ (1,3) $ - $ (1,3) $