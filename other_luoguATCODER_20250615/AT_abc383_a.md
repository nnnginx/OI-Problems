# AT_abc383_a [ABC383A] Humidifier 1

## 题目描述

AtCoder 公司办公室有一个加湿器。当前时间是 $0$ ，加湿器内没有水。

你要给加湿器加水 $N$ 次。第 $i$ 次加水（ $1 \leq i \leq N$ ）发生在时间 $T_i$ ，您加了 $V_i$ 升水。保证所有 $1 \leq i \leq N-1$ 的 $T_i < T_{i+1}$ 。

然而，加湿器漏水了，只要里面有水，单位时间内水量就会减少 $1$ 升。

求在 $T_N$ 时加完水后加湿器中剩余的水量。

## 输入格式

从标准输入读入，格式如下


>$N$
$T_1$ $V_1$
$T_2$ $V_2$
$\vdots$
$T_N$ $V_N$

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
4
1 3
3 1
4 4
7 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3
1 8
10 11
21 5
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
10
2 1
22 10
26 17
29 2
45 20
47 32
72 12
75 1
81 31
97 7
```

### 输出 #3

```
57
```

## 说明/提示

### 限制

- $1 \leq N \leq 100$
- $1 \leq T_i \leq 100$ ( $1 \leq i \leq N$ )
- $1 \leq V_i \leq 100$ ( $1 \leq i \leq N$ )
- $T_i < T_{i+1}$ ( $1 \leq i \leq N-1$ )
- 所有输入值均为整数。

### 样例解释1

每个时间点的加水量如下：

- 时间 $1$ ：加水前，加湿器有 $0$ 升水。添加 $3$ 升水后，加湿器有 $3$ 升水。
- 时间 $3$ ：添加前有 $1$ 升。添加 $1$ 升后，它的总容量为 $2$ 升。
- 时间 $4$ ：加水前有 $1$ 升。添加 $4$ 升后，总计有 $5$ 升。
- 时间 $7$ ：添加前有 $2$ 升。添加 $1$ 升后，总计有 $3$ 升。

在 $7$ 时完成添加后，加湿器有 $3$ 升。因此，答案为 $3$ 。

翻译提供者：[Willson1307](https://www.luogu.com.cn/user/1016880)