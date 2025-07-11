# AT_agc005_d [AGC005D] ~K Perm Counting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_d

すぬけ君は順列が大好きなので、長さ $ N $ の順列を作ることにしました。

ただしすぬけ君は整数 $ K $ が嫌いなので、以下の条件を満たす順列を作ることにしました。

- 順列を $ a_1,\ a_2,\ ...,\ a_N $ とする。全ての $ i\ =\ 1,2,...,N $ について、$ |a_i\ -\ i|\ \neq\ K $ を満たす

長さ $ N $ の順列は $ N! $ 通りありますが、そのうち条件をみたすものは何個あるかを求めてください。

ただし答えは非常に大きくなることがあるので、答えを $ 924844033 $(素数) で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式

$ 1 $ 行に答えを $ 924844033 $ で割ったあまりを出力する。

## 输入输出样例 #1

### 输入 #1

```
3 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4 1
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
4 2
```

### 输出 #3

```
9
```

## 输入输出样例 #4

### 输入 #4

```
4 3
```

### 输出 #4

```
14
```

## 输入输出样例 #5

### 输入 #5

```
425 48
```

### 输出 #5

```
756765083
```

## 说明/提示

### 制約

- $ 2\ ≦\ N\ ≦\ 2000 $
- $ 1\ ≦\ K\ ≦\ N-1 $

### Sample Explanation 1

$ (1,\ 2,\ 3) $, $ (3,\ 2,\ 1) $ の $ 2 $ つが条件を満たす。

### Sample Explanation 2

$ (1,\ 2,\ 3,\ 4) $, $ (1,\ 4,\ 3,\ 2) $, $ (3,\ 2,\ 1,\ 4) $, $ (3,\ 4,\ 1,\ 2) $, $ (4,\ 2,\ 3,\ 1) $ の $ 5 $ つが条件を満たす。