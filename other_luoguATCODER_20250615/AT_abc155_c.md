# AT_abc155_c [ABC155C] Poll

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc155/tasks/abc155_c

$ N $ 枚の投票用紙があり、$ i\ (1\ \leq\ i\ \leq\ N) $ 枚目には文字列 $ S_i $ が書かれています。

書かれた回数が最も多い文字列を全て、辞書順で小さい順に出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ : $ $ S_N $

## 输出格式

あてはまる文字列を全て辞書順で小さい順に、改行区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7
beat
vet
beet
bed
vet
bet
beet
```

### 输出 #1

```
beet
vet
```

## 输入输出样例 #2

### 输入 #2

```
8
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
```

### 输出 #2

```
buffalo
```

## 输入输出样例 #3

### 输入 #3

```
7
bass
bass
kick
kick
bass
kick
kick
```

### 输出 #3

```
kick
```

## 输入输出样例 #4

### 输入 #4

```
4
ushi
tapu
nichia
kun
```

### 输出 #4

```
kun
nichia
tapu
ushi
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ S_i $ は英小文字のみからなる文字列 $ (1\ \leq\ i\ \leq\ N) $
- $ S_i $ の長さは $ 1 $ 以上 $ 10 $ 以下 $ (1\ \leq\ i\ \leq\ N) $

### Sample Explanation 1

書かれた回数は `beet` と `vet` が $ 2 $ 回、`beat` と `bed` と `bet` が $ 1 $ 回です。したがって、$ 2 $ 回書かれた `beet` と `vet` を出力します。