# AT_abc393_e [ABC393E] GCD of Subset

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc393/tasks/abc393_e

给定一个长度为 $ N $ 的数列 $ A=(A_1,A_2,\dots,A_N) $ 和一个不超过 $ N $ 的正整数 $ K $。  
对于每个 $ i=1,2,\dots,N $，请解决以下问题：

- 从 $ A $ 中选出包含 $ A_i $ 的 $ K $ 个元素时，求这些元素的最大公约数 (GCD) 可能达到的最大值。

## 输入格式

输入通过标准输入给出，格式如下：

> $ N $ $ K $  
> $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式

输出 $ N $ 行。第 $ j $ 行应输出 $ i=j $ 时的答案。

## 输入输出样例 #1

### 输入 #1

```
5 2
3 4 6 7 12
```

### 输出 #1

```
3
4
6
1
6
```

## 输入输出样例 #2

### 输入 #2

```
3 3
6 10 15
```

### 输出 #2

```
1
1
1
```

## 输入输出样例 #3

### 输入 #3

```
10 3
414003 854320 485570 52740 833292 625990 909680 885153 435420 221663
```

### 输出 #3

```
59
590
590
879
879
590
20
879
590
59
```

## 说明/提示

### 约束条件

- $ 1 \leq K \leq N \leq 1.2 \times 10^6 $
- $ 1 \leq A_i \leq 10^6 $
- 输入中所有值均为整数

### 样例解释 1

- 当 $ i=1 $ 时，选择 $ A_1 $ 和 $ A_3 $，最大公约数为 $\gcd(\{3, 6\}) = 3$，这是最大值。
- 当 $ i=2 $ 时，选择 $ A_2 $ 和 $ A_5 $，最大公约数为 $\gcd(\{4, 12\}) = 4$，这是最大值。
- 当 $ i=3 $ 时，选择 $ A_3 $ 和 $ A_5 $，最大公约数为 $\gcd(\{6, 12\}) = 6$，这是最大值。
- 当 $ i=4 $ 时，选择 $ A_4 $ 和 $ A_2 $，最大公约数为 $\gcd(\{7, 4\}) = 1$，这是最大值。
- 当 $ i=5 $ 时，选择 $ A_5 $ 和 $ A_3 $，最大公约数为 $\gcd(\{12, 6\}) = 6$，这是最大值。

翻译由 DeepSeek R1 完成