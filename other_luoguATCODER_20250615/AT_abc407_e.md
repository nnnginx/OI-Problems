# AT_abc407_e [ABC407E] Most Valuable Parentheses

## 题目描述

给你一个长度为 $2N$ 的数列 $A$。

定义一个长度为 $2N$ 的括号序列 $s$ 的得分：

- 对于所有 $s_i=$`)`，$A_i\leftarrow 0$；
- 得分为上述操作后 $A$ 中所有元素之和。

请求出对于一个长为 $2N$ 的合法的括号序列 $s$，它的得分的最大值。一个括号序列是合法的当且仅当它可以通过多次删去子段 `()` 变为空串。

## 输入格式

多组数据。第一行一个整数 $T(1\le T\le 500)$ 表示数据组数。

对于每组数据：\
第一行一个整数 $N(1\le N\le 2\times 10^5)$。\
接下来 $2N$ 行，每行一个数字，依次为 $A_1,A_2,\cdots,A_{2N}(0\le A_i\le 10^9)$。

保证单个测试点内 $\sum N\le 2\times 10^5$。

## 输出格式

对于每组数据，输出一行一个整数表示答案。***

## 输入输出样例 #1

### 输入 #1

```
2
3
400
500
200
100
300
600
6
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
```

### 输出 #1

```
1200
6000000000
```

## 说明/提示

**样例解释 1**

在第一组数据中，$s=$`(())()` 的得分为 $400+500+0+0+300+0=1200$。可以证明这是可能获得的最大的分，故答案为 $1200$。

如第二组数据所示，答案可能超出 32 位整数的表示范围。

By @[chenxi2009](/user/1020063)