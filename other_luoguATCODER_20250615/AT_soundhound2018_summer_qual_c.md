# AT_soundhound2018_summer_qual_c Ordinary Beauty

## 题目描述

[problemUrl]: https://atcoder.jp/contests/soundhound2018-summer-qual/tasks/soundhound2018_summer_qual_c

数列 $ (a_1,...\ ,a_n) $ の *美しさ* を、隣り合う $ 2 $ 項の組であって、 差の絶対値が $ d $ であるものの個数として定義します。 例えば、$ d=1 $ であるとき、数列 $ (3,\ 2,\ 3,\ 10,\ 9) $ の美しさは $ 3 $ です。

各要素が $ 1 $ 以上 $ n $ 以下の整数である長さ $ m $ の数列は全部で $ n^m $ 通り存在します。 この $ n^m $ 通りの数列すべてに対して美しさを求めて、 それらの平均を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ n $ $ m $ $ d $

## 输出格式

各要素が $ 1 $ 以上 $ n $ 以下の整数である長さ $ m $ の数列 の美しさの平均を出力せよ。 絶対誤差または相対誤差が $ 10^{-6} $ 以下ならば正解となる。

## 输入输出样例 #1

### 输入 #1

```
2 3 1
```

### 输出 #1

```
1.0000000000
```

## 输入输出样例 #2

### 输入 #2

```
1000000000 180707 0
```

### 输出 #2

```
0.0001807060
```

## 说明/提示

### 制約

- $ 0\ \leq\ d\ <\ n\ \leq\ 10^9 $
- $ 2\ \leq\ m\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

$ (1,1,1) $ の美しさは $ 0 $ です。 $ (1,1,2) $ の美しさは $ 1 $ です。 $ (1,2,1) $ の美しさは $ 2 $ です。 $ (1,2,2) $ の美しさは $ 1 $ です。 $ (2,1,1) $ の美しさは $ 1 $ です。 $ (2,1,2) $ の美しさは $ 2 $ です。 $ (2,2,1) $ の美しさは $ 1 $ です。 $ (2,2,2) $ の美しさは $ 0 $ です。 これらの平均である、 $ (0+1+2+1+1+2+1+0)/8=1 $ が答えとなります。