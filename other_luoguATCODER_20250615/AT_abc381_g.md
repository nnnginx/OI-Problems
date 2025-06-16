# AT_abc381_g [ABC381G] Fibonacci Product

## 题目描述

# [ABC381G] 斐波那契积

## 问题描述

[problemUrl]: https://atcoder.jp/contests/abc381/tasks/abc381_g

定义数列 $ a_1,\ a_2,\ a_3,\ \dots $ 的通项公式如下：

$$ a_n\ =\ \begin{cases}x\ \ &(n=1)\ \\ y\ \ &(n=2)\ \\ a_{n-1}\ +\ a_{n-2}\ \ &(n\geq 3)\ \\ \end{cases} $$ 

请计算 $ \left(\displaystyle\ \prod_{i=1}^N\ a_i\right)\ \bmod{998244353} $。

本题多测，给定 $ T $ 组数据，请你对每一组数据求解。

## 输入格式

输入以以下形式从标准输入给出，其中 $ \mathrm{case}_i $ 表示第 $ i $ 个测试用例。

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \dots $ $ \mathrm{case}_{T} $

每个测试用例按以下形式给出：

> $ N $ $ x $ $ y $

## 输出格式

输出 $ T $ 行。第 $ i $ 行输出第 $ i $ 组数据的答案。

## 输入输出样例 #1

### 输入 #1

```
3
5 1 1
2024 11 22
1000000000000000000 12345 6789
```

### 输出 #1

```
30
577322229
726998219
```

## 说明/提示

### 限制条件

- $ 1\ \leq\ T\ \leq\ 5 $
- $ 1\ \leq\ N\ \leq\ 10^{18} $
- $ 0\ \leq\ x\ \leq\ 998244352 $
- $ 0\ \leq\ y\ \leq\ 998244352 $
- 输入的所有值均为整数

### 样例解释 1

对于第 $ 1 $ 个测试用例，数列的各项为 $ 1,\ 1,\ 2,\ 3,\ 5,\ 8,\ \dots $。因此，$ (1\ \times\ 1\ \times\ 2\ \times\ 3\ \times\ 5)\ \bmod{998244353}\ =\ 30 $ 为答案。