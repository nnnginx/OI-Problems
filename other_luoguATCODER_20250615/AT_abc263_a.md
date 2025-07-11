# AT_abc263_a [ABC263A] Full House

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc263/tasks/abc263_a

$ 5 $ 枚のカードがあり、それぞれのカードには整数 $ A,B,C,D,E $ が書かれています。

この $ 5 $ 枚組は以下の条件を満たすとき、またそのときに限って、フルハウスであると呼ばれます。

- 同じ数が書かれたカード $ 3 $ 枚と、別の同じ数が書かれたカード $ 2 $ 枚からなる。

$ 5 $ 枚組がフルハウスであるか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $ $ E $

## 输出格式

フルハウスである場合 `Yes` を、そうでないとき `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 2 1 2 1
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
12 12 11 1 2
```

### 输出 #2

```
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ A,B,C,D,E\leq\ 13 $
- $ A,B,C,D,E $ 全てが同じ値ではない
- 入力は全て整数

### Sample Explanation 1

$ 1 $ が書かれたカード $ 3 $ 枚と、$ 2 $ が書かれたカード $ 2 $ 枚からなるため、これはフルハウスです。

### Sample Explanation 2

フルハウスの条件を満たしません。