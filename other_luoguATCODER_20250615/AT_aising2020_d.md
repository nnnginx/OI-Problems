# AT_aising2020_d Anything Goes to Zero

## 题目描述

# 任何东西都会归零
[problemUrl]: https://atcoder.jp/contests/aising2020/tasks/aising2020_d
定义 $ \mathrm{popcount}(n) $ 为 $ n $ 在二进制表示中 '1' 的个数。例如，$ \mathrm{popcount}(3)\ =\ 2,\ \mathrm{popcount}(7)\ =\ 3,\ \mathrm{popcount}(0)\ =\ 0 $。
定义 $ f(n) $ 为将 $ n $ 用 $ \mathrm{popcount}(n) $ 除后取余数替换 $ n $ 的操作次数，直到 $ n $ 变为 $ 0 $ 为止（在这个问题的约束下，可以证明 $ n $ 经过有限次操作后一定会变为 $ 0 $）。
以下是以 $ n=7 $ 为例，经过 2 次操作 $ n $ 变为 0 的过程。
- 因为 $ \mathrm{popcount}(7)=3 $，所以用 3 除 7 后的余数 1 替换 7。
- 因为 $ \mathrm{popcount}(1)=1 $，所以用 1 除 1 后的余数 0 替换 1。
给定一个二进制表示的 $ N $ 位整数 $ X $。对于满足 $ 1\ \leq\ i\ \leq\ N $ 的整数 $ i $，定义将 $ X $ 的第 $ i $ 位取反后的整数为 $ X_i $。求 $ f(X_1),\ f(X_2),\ \ldots,\ f(X_N) $。

## 输入格式

输入从标准输入中以以下形式给出。
> $ N $ $ X $

## 输出格式

输出 $ N $ 行。第 $ i $ 行输出 $ f(X_i) $ 的值。
## 样例 #1
### 样例输入 #1
```
3
011
```
### 样例输出 #1
```
2
1
1
```
## 样例 #2
### 样例输入 #2
```
23
00110111001011011001110
```
### 样例输出 #2
```
2
1
2
2
1
2
2
2
2
2
2
2
2
2
2
2
2
2
2
2
2
1
3
```

## 输入输出样例 #1

### 输入 #1

```
3
011
```

### 输出 #1

```
2
1
1
```

## 输入输出样例 #2

### 输入 #2

```
23
00110111001011011001110
```

### 输出 #2

```
2
1
2
2
1
2
2
2
2
2
2
2
2
2
2
2
2
2
2
2
2
1
3
```

## 说明/提示

### 制約
- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ X $ 是二进制表示的 $ N $ 位的整数（首位不一定是 '1'）
### 样例解释 #1
- $ X_1 $ 是 7。因为 7 变为 1 再变为 0，所以 $ f(7) = 2 $。
- $ X_2 $ 是 1。因为 1 变为 0，所以 $ f(1) = 1 $。
- $ X_3 $ 是 2。因为 2 变为 0，所以 $ f(2) = 1 $。