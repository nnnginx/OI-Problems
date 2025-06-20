# AT_abc247_g [ABC247G] Dream Team

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc247/tasks/abc247_g

$ N $ 人の競技プログラマがいます。  
 $ i $ 人目の競技プログラマは、所属大学が $ A_i $、得意分野が $ B_i $、強さが $ C_i $ です。

$ N $ 人のうちの何人かによって構成されるチームであって、次の条件をともに満たすものを**ドリームチーム**と呼びます。

- チームに属するどの $ 2 $ 人の所属大学も異なる
- チームに属するどの $ 2 $ 人の得意分野も異なる

構成可能なドリームチームの人数の最大値を $ k $ とします。各 $ i=1,2,\ldots,k $ について、次の問題を解いてください。

問題：ちょうど $ i $ 人で構成されるドリームチームについて、チームに所属する人の強さの合計の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ C_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ \vdots $ $ A_N $ $ B_N $ $ C_N $

## 输出格式

構成可能なドリームチームの人数の最大値を $ k $ とする。  
 1行目には $ k $ を出力し、その後、$ k $ 行にわたって、$ i=1,2,\ldots,k $ のときの問題に対する答えを順に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 1 100
1 20 10
2 1 1
```

### 输出 #1

```
2
100
11
```

## 输入输出样例 #2

### 输入 #2

```
10
1 4 142135623
2 6 457513110
3 1 622776601
5 1 961524227
2 2 360679774
2 4 494897427
3 7 416573867
5 2 915026221
1 7 320508075
5 3 851648071
```

### 输出 #2

```
4
961524227
1537802822
2032700249
2353208324
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 3\times\ 10^4 $
- $ 1\ \leq\ A_i,B_i\ \leq\ 150 $
- $ 1\ \leq\ C_i\ \leq\ 10^9 $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

\- ちょうど $ 1 $ 人で構成されるドリームチームは、$ 1 $ 人目の競技プログラマからなるとき強さの合計が $ 100 $ で最大になります。 - ちょうど $ 2 $ 人で構成されるドリームチームは、$ 2,3 $ 人目の競技プログラマからなるとき強さの合計が $ 11 $ で最大になります。 - ちょうど $ 3 $ 人で構成されるドリームチームを作ることはできません。