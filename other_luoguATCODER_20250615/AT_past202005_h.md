# AT_past202005_h ハードル走

## 题目描述

有一个人在数轴原点处。他每 $t_1$ 秒跑 $1$ 个单位长度，每 $t_2$ 秒跳一个单位长度。

在数轴上有 $n$ 个点放了障碍物，左起第 $i$ 个放置障碍物的点表示的数为 $x_i$。

他每次行动可以从下面的三种行动中选择一种执行：

1. 跑 $1$ 个单位长度；
1. 跑 $0.5$ 个单位长度，跳 $1$ 个单位长度，再跑 $0.5$ 个单位长度，共行进 $2$ 个单位长度；
1. 跑 $0.5$ 个单位长度，跳 $3$ 个单位长度，再跑 $0.5$ 个单位长度，共行进 $4$ 个单位长度；

若这个人在通过一个障碍点时不在空中，那么他需要额外花 $t_3$ 秒通过。

请求出：这个人到达表示数 $l$ 的点至少需要多少秒？（如果是跳过去的，考虑他在空中经过该点的时间）

## 输入格式

输入共 $3$ 行。

第一行：两个整数 $n,l$。

第二行：$n$ 个整数 $x_1,x_2,...,x_n$。

第三行：三个整数 $t_1,t_2,t_3$。

## 输出格式

输出此人通过表示数 $l$ 的点的时间。保证结果为整数。

### 数据规模与约定

- $2 \le l \le 10^5$，$1\le n \lt l$；
- $0 \lt x_i \lt l$，且 $x_i$ 单调递增；
- $2 \le t_1,t_2,t_3 \le 1000$，且它们均为偶数。

## 输入输出样例 #1

### 输入 #1

```
2 5
1 4
2 2 20
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
4 5
1 2 3 4
2 20 100
```

### 输出 #2

```
164
```

## 输入输出样例 #3

### 输入 #3

```
10 19
1 3 4 5 7 8 10 13 15 17
2 1000 10
```

### 输出 #3

```
138
```