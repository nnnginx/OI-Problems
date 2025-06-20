# AT_abc251_c [ABC251C] Poem Online Judge

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc251/tasks/abc251_c

ポエムオンラインジャッジ (Poem Online Judge, 以下 POJ と表記) は提出された文字列に得点をつけるオンラインジャッジです。  
 POJ に $ N $ 回の提出がありました。早い方から $ i $ 番目の提出では文字列 $ S_i $ が提出されて、得点は $ T_i $ でした。(同じ文字列が複数回提出される場合もあります)  
 ただし、POJ では **同じ文字列を提出しても得点が等しいとは限らない** のに注意してください。

$ N $ 回の提出のうち、その提出よりも早い提出であって文字列が一致するものが存在しないような提出を **オリジナル** であると呼びます。  
 また、オリジナルな提出の中で最も得点が高いものを **最優秀賞** と呼びます。ただし、そのような提出が複数ある場合は、最も提出が早いものを最優秀賞とします。

最優秀賞は早い方から何番目の提出ですか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ T_1 $ $ S_2 $ $ T_2 $ $ \vdots $ $ S_N $ $ T_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
aaa 10
bbb 20
aaa 30
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5
aaa 9
bbb 10
ccc 10
ddd 10
bbb 11
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
10
bb 3
ba 1
aa 4
bb 1
ba 5
aa 9
aa 2
ab 6
bb 5
ab 3
```

### 输出 #3

```
8
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ S_i $ は英小文字からなる文字列
- $ S_i $ の長さは $ 1 $ 以上 $ 10 $ 以下
- $ 0\ \leq\ T_i\ \leq\ 10^9 $
- $ N $, $ T_i $ は整数

### Sample Explanation 1

以下では早い方から $ i $ 番目の提出を提出 $ i $ と呼びます。 オリジナルな提出は提出 $ 1 $ と 提出 $ 2 $ です。提出 $ 3 $ は提出 $ 1 $ と文字列が一致しているためオリジナルではありません。 オリジナルな提出のうち最も得点が高い提出は提出 $ 2 $ です。よってこれが最優秀賞になります。

### Sample Explanation 2

オリジナルな提出は提出 $ 1 $・提出 $ 2 $・提出 $ 3 $・提出 $ 4 $ です。 その中で最も得点が高い提出は提出 $ 2 $・提出 $ 3 $・提出 $ 4 $ です。この場合はこの中でもっとも提出の早い提出 $ 2 $ を最優秀賞とします。 このように、オリジナルな提出の中で最も得点が高い提出が複数ある場合は、さらにその中で最も提出が早いものを最優秀賞とするのに注意してください。