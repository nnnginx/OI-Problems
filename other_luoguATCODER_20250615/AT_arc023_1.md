# AT_arc023_1 [ARC023A] 经过天数

## 题目描述

给定一个日期，求出该日期与 $2014$ 年 $5$ 月 $17$ 日相差的天数。

下面的公式可以求出 $y$ 年 $m$ 月 $d$ 日与 $1$ 年 $1$ 月 $1$ 日相差的天数：

$$365y + \lfloor \dfrac{y}{4} \rfloor - \lfloor \dfrac{y}{100} \rfloor + \lfloor \dfrac{y}{400} \rfloor + \lfloor \dfrac{306(m + 1)}{10} \rfloor + d - 429$$

其中 $\lfloor x \rfloor$ 表示对 $x$ 向下取整，例如 $\lfloor 1.5 \rfloor = 1$，$\lfloor 2.0 \rfloor = 2$。

特别地，如果月份为 $1$ 月或 $2$ 月，则应用上述公式时需要换成前一年的 $13$ 月或 $14$ 月。例如 $2012$ 年 $2$ 月 $5$ 日需要代入 $y = 2011,m = 14,d = 5$。

## 输入格式

输入数据共有三行，每行一个整数，分别为 $y,m,d$。

## 输出格式

输出一行一个整数，表示所求的答案。

## 输入输出样例 #1

### 输入 #1

```
1988
7
3
```

### 输出 #1

```
9449
```

## 输入输出样例 #2

### 输入 #2

```
1
1
1
```

### 输出 #2

```
735369
```

## 输入输出样例 #3

### 输入 #3

```
2014
5
16
```

### 输出 #3

```
1
```

## 输入输出样例 #4

### 输入 #4

```
2012
2
29
```

### 输出 #4

```
808
```

## 说明/提示

所有数据保证 $1\leq y\leq2014$，$1\leq m\leq 12$，$1\leq d\leq 31$，对应的日期在 $2014$ 年 $5$ 月 $17$ 日之前，且为现实中真实存在的日期。