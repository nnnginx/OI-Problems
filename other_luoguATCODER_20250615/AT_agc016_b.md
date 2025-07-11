# AT_agc016_b [AGC016B] Colorful Hats

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc016/tasks/agc016_b

$ N $ 匹の猫がいます。 猫には $ 1 $ から $ N $ まで番号が振られています。

各猫はある色の帽子を被っています。 猫 $ i $ は「自分を除く $ N-1 $ 匹の猫が被っている帽子の色の種類数はちょうど $ a_i $ である」と言っています。

すべての猫の発言と矛盾しないような帽子の色の組合せが存在するか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式

すべての猫の発言と矛盾しないような帽子の色の組合せが存在するならば、`Yes` を出力せよ。 存在しないならば、`No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 2 2
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
3
1 1 2
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
5
4 3 4 3 4
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
3
2 2 2
```

### 输出 #4

```
Yes
```

## 输入输出样例 #5

### 输入 #5

```
4
2 2 2 2
```

### 输出 #5

```
Yes
```

## 输入输出样例 #6

### 输入 #6

```
5
3 3 3 3 3
```

### 输出 #6

```
No
```

## 说明/提示

### 制約

- $ 2\ <\ =\ N\ <\ =\ 10^5 $
- $ 1\ <\ =\ a_i\ <\ =\ N-1 $

### Sample Explanation 1

例えば、猫 $ 1 $, $ 2 $, $ 3 $ の帽子の色がそれぞれ赤、青、青ならば、すべての猫の発言と矛盾しません。

### Sample Explanation 2

猫 $ 1 $ の発言から、猫 $ 2 $, $ 3 $ の帽子の色は同一です。 また、猫 $ 2 $ の発言から、猫 $ 1 $, $ 3 $ の帽子の色は同一です。 よって、猫 $ 1 $, $ 2 $ の帽子の色は同一ですが、これは猫 $ 3 $ の発言に矛盾します。