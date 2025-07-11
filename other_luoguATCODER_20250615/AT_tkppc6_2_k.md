# AT_tkppc6_2_k Ball in the Box 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tkppc6-2/tasks/tkppc6_2_k

かめ君は $ N $ 種類の色のついたボールを持っています。

色には $ 1,\ 2,\ \ldots\ ,\ N $ と番号が振られており、各整数 $ i\ (1\ \le\ i\ \le\ N) $ について色 $ i $ のついたボールは $ A_i $ 個あります。

各整数 $ k\ =\ 1,\ 2,\ \ldots\ ,\ M $ に対し、以下の値を $ 998244353 $ で割ったあまりをそれぞれ出力してください。

- 互いに区別できる $ k $ 個の箱に、持っているすべてのボールを入れるときのボールの入れ方の総数（ここで、ボールが一つも入っていない箱があってもよい）

ただし、ある箱とある正整数 $ i $ が存在して、その箱に入っている色 $ i $ のボールの個数が異なるとき、またそのときに限りボールの入れ方が異なるとみなします（つまり、同じ色のボールは区別しません）。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

$ M $ 行出力せよ。 $ i $ 行目には、 $ k\ =\ i $ の時の答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2
1 2 3
```

### 输出 #1

```
1
24
```

## 输入输出样例 #2

### 输入 #2

```
2 3
1 1
```

### 输出 #2

```
1
4
9
```

## 输入输出样例 #3

### 输入 #3

```
4 5
31415 92653 58979 32384
```

### 输出 #3

```
1
287242452
806145507
819893815
181831825
```

## 说明/提示

### 制約

- $ 1\ \le\ N\ \le\ 250000 $
- $ 1\ \le\ M\ \le\ 100000 $
- $ 1\ \le\ A_i\ <\ 998244353\ (1\ \le\ i\ \le\ N) $
- 入力は全て整数

### Sample Explanation 1

色 $ 1 $ のボールは $ 1 $ 個、色 $ 2 $ のボールは $ 2 $ 個、色 $ 3 $ のボールは $ 3 $ 個あります。 $ k=2 $ の時、一方の箱に何個のボールを入れるかを決めればもう片方に入れるボールの数が決まるため、答えは $ 2\ \times\ 3\ \times\ 4\ =\ 24 $ となります。

### Sample Explanation 3

$ 998244353 $ で割った余りを出力することに注意してください。 原案: \[turtle0123\\\_\\\_\](https://atcoder.jp/users/turtle0123\_\_)