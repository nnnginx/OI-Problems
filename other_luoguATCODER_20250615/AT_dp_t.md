# AT_dp_t Permutation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_t

$ N $ を正整数とします。 長さ $ N\ -\ 1 $ の文字列 $ s $ が与えられます。 $ s $ は `<` と `>` からなります。

$ (1,\ 2,\ \ldots,\ N) $ を並べ替えた順列 $ (p_1,\ p_2,\ \ldots,\ p_N) $ であって、次の条件を満たすものは何通りでしょうか？ $ 10^9\ +\ 7 $ で割った余りを求めてください。

- 各 $ i $ ($ 1\ \leq\ i\ \leq\ N\ -\ 1 $) について、$ s $ の $ i $ 文字目が `<` の場合は $ p_i\ <\ p_{i\ +\ 1} $ であり、$ s $ の $ i $ 文字目が `>` の場合は $ p_i\ >\ p_{i\ +\ 1} $ である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ s $

## 输出格式

条件を満たす順列は何通りか？ $ 10^9\ +\ 7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
<><
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
5
<<<<
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
20
>>>><>>><>><>>><<>>
```

### 输出 #3

```
217136290
```

## 说明/提示

### 制約

- $ N $ は整数である。
- $ 2\ \leq\ N\ \leq\ 3000 $
- $ s $ は長さ $ N\ -\ 1 $ の文字列である。
- $ s $ は `<` と `>` からなる。

### Sample Explanation 1

条件を満たす順列は次の $ 5 $ 通りです。 - $ (1,\ 3,\ 2,\ 4) $ - $ (1,\ 4,\ 2,\ 3) $ - $ (2,\ 3,\ 1,\ 4) $ - $ (2,\ 4,\ 1,\ 3) $ - $ (3,\ 4,\ 1,\ 2) $

### Sample Explanation 2

条件を満たす順列は次の $ 1 $ 通りです。 - $ (1,\ 2,\ 3,\ 4,\ 5) $

### Sample Explanation 3

答えを $ 10^9\ +\ 7 $ で割った余りを出力することを忘れずに。