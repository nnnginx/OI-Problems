# AT_abc312_a [ABC312A] Chord

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc312/tasks/abc312_a

英大文字からなる長さ $ 3 $ の文字列 $ S $ が与えられます。$ S $ が `ACE`、`BDF`、`CEG`、`DFA`、`EGB`、`FAC`、`GBD` のいずれかと等しいとき `Yes` を、そうでないとき `No` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ S $ が `ACE`、`BDF`、`CEG`、`DFA`、`EGB`、`FAC`、`GBD` のいずれかと等しいとき `Yes` を、そうでないとき `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
ABC
```

### 输出 #1

```
No
```

## 输入输出样例 #2

### 输入 #2

```
FAC
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
XYX
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ S $ は英大文字からなる長さ $ 3 $ の文字列
 
### Sample Explanation 1

$ S\ = $ `ABC` のとき、$ S $ は `ACE`、`BDF`、`CEG`、`DFA`、`EGB`、`FAC`、`GBD` のいずれとも等しくないので `No` を出力します。