# AT_abc083_a [ABC083A] Libra

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc083/tasks/abc083_a

上皿天秤は、左の皿に乗っているおもりの重さの合計を $ L $ とし、右の皿に乗っているおもりの重さの合計を $ R $ としたとき、 $ L\ >\ R $ なら左に傾き、$ L=R $ なら釣り合い、$ L\ <\ R $ なら右に傾きます。

高橋君は、上皿天秤の左の皿に重さ $ A $ のおもりと重さ $ B $ のおもりを、右の皿に重さ $ C $ のおもりと重さ $ D $ のおもりを置きました。

上皿天秤が左に傾くなら `Left` を、釣り合うなら `Balanced` を、右に傾くなら `Right` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $

## 输出格式

上皿天秤が左に傾くなら `Left` を、釣り合うなら `Balanced` を、右に傾くなら `Right` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 8 7 1
```

### 输出 #1

```
Left
```

## 输入输出样例 #2

### 输入 #2

```
3 4 5 2
```

### 输出 #2

```
Balanced
```

## 输入输出样例 #3

### 输入 #3

```
1 7 6 4
```

### 输出 #3

```
Right
```

## 说明/提示

### 制約

- $ 1\leq\ A,B,C,D\ \leq\ 10 $
- 入力はすべて整数である

### Sample Explanation 1

左の皿の上のおもりの重さの合計は $ 11 $ 、右の皿の上のおもりの重さの合計は $ 8 $ です。$ 11\ >\ 8 $ なので、`Left` を出力します。

### Sample Explanation 2

左の皿の上のおもりの重さの合計は $ 7 $ 、右の皿の上のおもりの重さの合計は $ 7 $ です。$ 7=7 $ なので、`Balanced` を出力します。

### Sample Explanation 3

左の皿の上のおもりの重さの合計は $ 8 $ 、右の皿の上のおもりの重さの合計は $ 10 $ です。$ 8\ <\ 10 $ なので、`Right` を出力します。