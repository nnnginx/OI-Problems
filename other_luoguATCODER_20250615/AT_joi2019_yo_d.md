# AT_joi2019_yo_d 日本沈没 (Japan Sinks)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2019yo/tasks/joi2019_yo_d

日本列島は細長い列島である．日本列島は平行な境界線により $ N $ 個の区画に分けられている．区画には端から順に $ 1 $ から $ N $ の番号が付けられている．区画 $ i $ ($ 1\ ≦\ i\ ≦\ N $) の高さは $ A_i $ である．

日本列島は海に囲まれており，海面の高さは場所によらず一定である．高さが海面の高さより高い区画を**陸地**と呼ぶ．

陸地が連続している部分のことを**島**と呼ぶ．より正確に書くと以下の通りである．整数 $ l $, $ r $ ($ 1\ ≦\ l\ ≦\ r\ ≦\ N $) について，日本列島のうち区画 $ l $，区画 $ l+1 $，$ ... $，区画 $ r $ からなる部分を**領域** \[$ l,\ r $\] という．以下の条件を満たす領域 \[$ l,\ r $\] を島という：

- 区画 $ l $，区画 $ l+1 $，$ ... $，区画 $ r $ はすべて陸地である．
- $ l\ >\ 1 $ ならば区画 $ l-1 $ は陸地ではない．
- $ r\ <\ N $ ならば区画 $ r+1 $ は陸地ではない．

海面の上昇により，日本列島は少しずつ沈没している．現在の海面の高さは $ 0 $ であるが，これは時間が経つにつれて徐々に上がり，ついには日本全体が海になってしまう．

JOI 君は，海面の高さが上昇すると，日本の島の数が増減することに気付いた．現在から，日本に陸地がなくなるまでの間 (現在も含む) における，島の数の最大値を求めたい．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

現在から，日本に陸地がなくなるまでの間 (現在も含む) における，島の数の最大値を 1 行で出力せよ．

## 输入输出样例 #1

### 输入 #1

```
6
0 1 2 1 3 2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6
3 2 3 0 2 0
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
10
4 1 2 1 2 3 5 4 3 2
```

### 输出 #3

```
3
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 100000\ (=\ 10^5) $
- $ 0\ ≦\ A_i\ ≦\ 1000000000\ (=\ 10^9) $ ($ 1\ ≦\ i\ ≦\ N $)

### 小課題

1. ($ 7 $ 点) $ N\ ≦\ 2000 $, $ A_i\ ≦\ 2000 $ ($ 1\ ≦\ i\ ≦\ N $)
2. ($ 8 $ 点) $ N\ ≦\ 2000 $
3. ($ 85 $ 点) 追加の制約はない．

### Sample Explanation 1

\- 海面の高さが $ 0 $ 以上 $ 1 $ 未満のとき，区画 $ 2,\ 3,\ 4,\ 5,\ 6 $ が陸地である．領域 \\\[$ 2,\ 6 $\\\] が唯一の島なので，島の数は $ 1 $ である． - 海面の高さが $ 1 $ 以上 $ 2 $ 未満のとき，区画 $ 3,\ 5,\ 6 $ が陸地である．領域 \\\[$ 3,\ 3 $\\\] と領域 \\\[$ 5,\ 6 $\\\] が島なので，島の数は $ 2 $ である． - 海面の高さが $ 2 $ 以上 $ 3 $ 未満のとき，区画 $ 5 $ のみが陸地である．領域 \\\[$ 5,\ 5 $\\\] が唯一の島なので，島の数は $ 1 $ である． - 海面の高さが $ 3 $ になると，陸地はなくなり，島の数は $ 0 $ になる． よって島の数の最大値は $ 2 $ なので，$ 2 $ を出力する．

### Sample Explanation 2

\- 海面の高さが $ 0 $ 以上 $ 2 $ 未満のとき，区画 $ 1,\ 2,\ 3,\ 5 $ が陸地である．領域 \\\[$ 1,\ 3 $\\\] と領域 \\\[$ 5,\ 5 $\\\] が島なので，島の数は $ 2 $ である． - 海面の高さが $ 2 $ 以上 $ 3 $ 未満のとき，区画 $ 1,\ 3 $ が陸地である．領域 \\\[$ 1,\ 1 $\\\] と領域 \\\[$ 3,\ 3 $\\\] が島なので，島の数は $ 2 $ である． - 海面の高さが $ 3 $ になると，陸地はなくなり，島の数は $ 0 $ になる． よって島の数の最大値は $ 2 $ なので，$ 2 $ を出力する．