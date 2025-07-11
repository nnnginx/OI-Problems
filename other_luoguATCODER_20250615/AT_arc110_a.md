# AT_arc110_a [ARC110A] Redundant Redundancy

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc110/tasks/arc110_a

整数 $ N $ があります。

$ 2,\ 3,\ \ldots,\ N $ のどれで割っても $ 1 $ 余る、$ N $ 以上 $ 10^{13} $ 以下の整数を $ 1 $ つ出力してください。

この問題の制約下では、そのような整数は必ず $ 1 $ つ以上存在します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

$ 2,\ 3,\ \ldots,\ N $ のどれで割っても $ 1 $ 余る、$ N $ 以上 $ 10^{13} $ 以下の整数を $ 1 $ つ出力せよ。

そのような整数が複数存在する場合、どれを出力しても構わない。

## 输入输出样例 #1

### 输入 #1

```
3
```

### 输出 #1

```
7
```

## 输入输出样例 #2

### 输入 #2

```
10
```

### 输出 #2

```
39916801
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 2\ \leq\ N\ \leq\ 30 $

### Sample Explanation 1

$ 7 $ を $ 2 $ で割った余りは $ 1 $、$ 7 $ を $ 3 $ で割った余りは $ 1 $ です。 $ 7 $ は $ 3 $ 以上 $ 10^{13} $ 以下の整数なので、条件を満たします。