# AT_abc153_b [ABC153B] Common Raccoon vs Monster

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc153/tasks/abc153_b

アライグマはモンスターと戦っています。

モンスターの体力は $ H $ です。

アライグマは $ N $ 種類の必殺技を使うことができ、$ i $ 番目の必殺技を使うとモンスターの体力を $ A_i $ 減らすことができます。 必殺技を使う以外の方法でモンスターの体力を減らすことはできません。

モンスターの体力を $ 0 $ 以下にすればアライグマの勝ちです。

アライグマが同じ必殺技を $ 2 $ 度以上使うことなくモンスターに勝つことができるなら `Yes` を、できないなら `No` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

アライグマが同じ必殺技を $ 2 $ 度以上使うことなくモンスターに勝つことができるなら `Yes` を、できないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 3
4 5 6
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
20 3
4 5 6
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
210 5
31 41 59 26 53
```

### 输出 #3

```
Yes
```

## 输入输出样例 #4

### 输入 #4

```
211 5
31 41 59 26 53
```

### 输出 #4

```
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ H\ \leq\ 10^9 $
- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^4 $
- 入力中のすべての値は整数である。

### Sample Explanation 1

例えば $ 2 $ 番目と $ 3 $ 番目の必殺技を使うことで、モンスターの体力を $ 0 $ 以下にできます。