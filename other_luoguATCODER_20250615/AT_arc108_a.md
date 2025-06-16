# AT_arc108_a [ARC108A] Sum and Product

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc108/tasks/arc108_a

整数 $ S,P $ が与えられます。 $ N+M=S,N\ \times\ M\ =P $ を満たすような正の整数の組 $ (N,M) $ はありますか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ P $

## 输出格式

$ N+M=S,N\ \times\ M\ =P $ を満たすような正の整数の組 $ (N,M) $ があるなら `Yes`、そうでないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
1000000000000 1
```

### 输出 #2

```
No
```

## 说明/提示

### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ S,P\ \leq\ 10^{12} $

### Sample Explanation 1

\- 例えば $ N=1,M=2 $ のとき、$ N+M=3,N\ \times\ M\ =2 $ となります。

### Sample Explanation 2

\- そのような $ (N,M) $ は存在しません。