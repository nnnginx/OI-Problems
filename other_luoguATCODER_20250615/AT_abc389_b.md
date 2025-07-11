# AT_abc389_b [ABC389B] tcaF

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc389/tasks/abc389_b

给定一个不小于 $ 2 $ 的整数 $ X $。

求满足 $ N! = X $ 的正整数 $ N $。

其中，$ N! $ 表示 $ N $ 的阶乘，且保证满足条件的 $ N $ 存在且唯一。

## 输入格式

输入通过标准输入给出，格式如下：

> $ X $

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
6
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
2432902008176640000
```

### 输出 #2

```
20
```

## 说明/提示

### 约束条件

- $ 2 \leq X \leq 3 \times 10^{18} $
- 满足 $ N! = X $ 的正整数 $ N $ 存在且唯一
- 输入均为整数

### 样例解释 1

因为 $ 3! = 3 \times 2 \times 1 = 6$，所以输出 3。

### 样例解释 2

因为 $ 20! = 2432902008176640000$，所以输出 20。

翻译由 DeepSeek R1 完成