# 三

## 题目背景

奶龙在小学学习了如何判断一个数是否是 $3$ 的倍数.

## 题目描述

多组数据.

每组数据给一个二进制正整数 $n$, 判断它是否是 $3$ 的倍数.

## 输入格式

第一行一个整数 $T$ 表示数据组数.

每组数据一行, 是一个仅包含 `0`, `1` 字符串 $S$. 从左到右从低到高地描述了 $S$ 的每个二进制位.

形式化地:

$$
N = \sum_{i = 0} 2^i[S_i == '1']
$$

保证没有前导零, 也就是说 $S$ 一定以 `1` 结尾.

## 输出格式

每组数据输出一行, 如果 $N$ 是 $3$ 的倍数则输出 `Yes`, 否则输出 `No`.

## 样例 #1

### 样例输入 #1

```
5
0101
1001
1
11
01
```

### 样例输出 #1

```
No
Yes
No
Yes
No
```

## 提示

对于 $20\%$ 的数据，$\lfloor \log n \rfloor \le 60$

对于 $60\%$ 的数据, $\lfloor \log n \rfloor \le 10000$

对于全部的数据， $\sum \lfloor \log n \rfloor \le 10000000$, $1 \leq n$, $T \le 100000$

请注意本题的空间限制.