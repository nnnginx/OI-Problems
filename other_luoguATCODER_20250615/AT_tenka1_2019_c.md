# AT_tenka1_2019_c Stones

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2019/tasks/tenka1_2019_c

$ N $ 個の石が一列に並んでおり、すべての石は白か黒で塗られています。 石の状態は長さ $ N $ の文字列 $ S $ で表され、$ S $ の $ i $ 文字目が `.` のとき左から $ i $ 個目の石が白であり、`#` のとき左から $ i $ 個目の石が黒であることを表します。

高橋君は、$ 0 $ 個以上の石の色を黒または白に変更し、黒い石のすぐ右に白い石があるような箇所がないようにしたいです。 色を変更する必要のある石の個数の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

色を変更する必要のある石の個数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
#.#
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
5
#.##.
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
9
.........
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ S $ は `.`, `#` のみからなる長さ $ N $ の文字列である

### Sample Explanation 1

例えば、$ 1 $ 個目の石の色を白に変更すればよいです。