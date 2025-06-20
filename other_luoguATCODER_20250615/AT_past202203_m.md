# AT_past202203_m ランキング

## 题目描述

维护一个长度为 $n$ 的数列 $p$。开始时，会按顺序给出 $p_i$ 的初始值。现在有 $q$ 次操作。

- `1 a x`：把 $p_a$ 的值改为 $x$。
- `2 a`：输出 $p_a$ 在数列中的排名（也就是求 $p_a$ 是整个数列中第几大的数）。
- `3 r`：输出数列中排名为 $r$ 的数的下标（也就是求整个数列中第 $r$ 大的数并输出其下标）。

数据保证每个 $p_i$ 和 $x$ 都不相同。

## 输入格式

第一行两个整数 $n,q$。

第二行 $n$ 个整数，表示数列 $p$。

后面 $q$ 行，每行一个询问（格式见题）。

## 输出格式

对于每个询问，输出一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
3 5
10 30 20
2 1
3 1
1 2 0
2 1
3 2
```

### 输出 #1

```
3
2
2
1
```

## 说明/提示

$1 \le n,q \le 5 \times 10^5$，$0 \le p_i,x \le 10^9$，$1 \le a,r \le n$。