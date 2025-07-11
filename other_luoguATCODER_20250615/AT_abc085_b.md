# AT_abc085_b [ABC085B] Kagami Mochi

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc085/tasks/abc085_b

*$ X $ 段重ねの鏡餅* $ (X\ >\ =\ 1) $ とは、$ X $ 枚の円形の餅を縦に積み重ねたものであって、どの餅もその真下の餅より直径が小さい（一番下の餅を除く）もののことです。例えば、直径 $ 10 $、$ 8 $、$ 6 $ センチメートルの餅をこの順に下から積み重ねると $ 3 $ 段重ねの鏡餅になり、餅を一枚だけ置くと $ 1 $ 段重ねの鏡餅になります。

ダックスフンドのルンルンは $ N $ 枚の円形の餅を持っていて、そのうち $ i $ 枚目の餅の直径は $ d_i $ センチメートルです。これらの餅のうち一部または全部を使って鏡餅を作るとき、最大で何段重ねの鏡餅を作ることができるでしょうか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ d_1 $ $ : $ $ d_N $

## 输出格式

作ることのできる鏡餅の最大の段数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
10
8
8
6
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3
15
15
15
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
7
50
30
50
100
50
80
30
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ <\ =\ N\ <\ =\ 100 $
- $ 1\ <\ =\ d_i\ <\ =\ 100 $
- 入力値はすべて整数である。

### Sample Explanation 1

直径 $ 10 $、$ 8 $、$ 6 $ センチメートルの餅をこの順に下から積み重ねると $ 3 $ 段重ねの鏡餅になり、これが最大です。

### Sample Explanation 2

すべての餅の直径が同じときは、$ 1 $ 段重ねの鏡餅しか作れません。