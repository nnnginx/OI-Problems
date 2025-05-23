## 奶龙算数

### 题目描述

小七拿来了一些数字来教奶龙算数。

奶龙面前总共有 $n$ 个数字。奶龙可以执行任意次以下两种操作：

1. 交给小七一块糖，拿走一个数字。
2. 交给小七 $a$ 块糖，拿走任意多个相同的数字。

奶龙想知道，拿走所有的数字至少要给小七几块糖，请你帮帮他。

### 输入格式

第一行，两个整数，$n, a$，分别表示数字的数量，操作 $2$ 所需的糖数 $a$；

第二行，$n$ 个整数，表示小七拿来的每个数字 $x_1,x_2, \cdots ,x_n$；

### 输出格式

共 $1$ 行，表示最少需要的糖的个数。

### 输入输出样例

#### 输入 #1

```
10 1
2 1 4 5 2 4 5 5 1 2
```

#### 输出 #1

```
4
```

#### 输入 #2

```
5 2
3 2 1 2 2
```

#### 输出 #2

```
4
```

### 说明 / 提示

#### 数据范围与约定

对于 $20\%$ 的数据，满足 $n \leq 20,a=1$.

对于另外 $20\%$ 的数据，满足 $a = 1$.

对于所有的数据，保证 $1\leq n,a,x_i \leq 100$.