# AT_abc177_d [ABC177D] Friends

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_d

人 $ 1 $ から 人 $ N $ までの $ N $ 人の人がいます。

「人 $ A_i $ と人 $ B_i $ は友達である」という情報が $ M $ 個与えられます。同じ情報が複数回与えられることもあります。

$ X $ と $ Y $ が友達、かつ、$ Y $ と $ Z $ が友達ならば、$ X $ と $ Z $ も友達です。また、$ M $ 個の情報から導くことができない友達関係は存在しません。

悪の高橋君は、この $ N $ 人をいくつかのグループに分け、全ての人について「同じグループの中に友達がいない」という状況を作ろうとしています。

最小でいくつのグループに分ければ良いでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_M $ $ B_M $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 3
1 2
3 4
5 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4 10
1 2
2 1
1 2
2 1
1 2
1 3
1 4
2 3
2 4
3 4
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
10 4
3 1
4 1
5 9
2 6
```

### 输出 #3

```
3
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 2\times\ 10^5 $
- $ 1\leq\ A_i,B_i\leq\ N $
- $ A_i\ \neq\ B_i $

### Sample Explanation 1

例えば $ \{1,3\},\{2,4\},\{5\} $ という $ 3 $ つのグループに分けることで目的を達成できます。