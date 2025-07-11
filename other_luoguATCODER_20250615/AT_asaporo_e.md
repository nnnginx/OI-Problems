# AT_asaporo_e 迷子の高橋君

## 题目描述

# 迷子の高橋君


青木君正试图寻找迷失在一次元世界中的高桥君。起初，青木君在坐标 $0$，而高桥君在坐标 $x$，之后，青木君无法得知高桥君的位置。

时间分为多个回合，每个回合以下操作同时进行：

- 青木君现在在坐标 $a$，可以选择移动到 $a-1$、$a$ 或 $a+1$。
- 高桥君现在在坐标 $b$，有 $p$ 百分比的概率移动到 $b-1$，有 $100-p$ 百分比的概率移动到 $b+1$。

当青木君和高桥君到达同一坐标时，青木君可以找到高桥君。若两者相遇但互相擦肩而过，青木君将无法找到高桥君。

青木君希望能最小化找到高桥君所需回合数的期望值。请计算该期望值。

## 输入格式

输入以以下格式提供：

> $x$ $p$

## 输出格式

输出期望值，要求绝对误差或相对误差在 $10^{-6}$ 以内。

## 示例 #1

### 示例输入 #1

```
3
100
```

### 示例输出 #1

```
2.0000000
```

## 示例 #2

### 示例输入 #2

```
6
40
```

### 示例输出 #2

```
7.5000000
```

## 示例 #3

### 示例输入 #3

```
101
80
```

### 示例输出 #3

```
63.7500000
```

## 输入输出样例 #1

### 输入 #1

```
3
100
```

### 输出 #1

```
2.0000000
```

## 输入输出样例 #2

### 输入 #2

```
6
40
```

### 输出 #2

```
7.5000000
```

## 输入输出样例 #3

### 输入 #3

```
101
80
```

### 输出 #3

```
63.7500000
```

## 说明/提示

### 约束条件

- $1 \leq x \leq 1,000,000,000$
- $1 \leq p \leq 100$
- $x$ 和 $p$ 均为整数。

### 部分得分

- 对于200个点的测试数据，$p=100$。
- 对于300个点的测试数据，$x \leq 10$。 

### 示例解释 #1

由于高桥君会必定向 $-1$ 移动，青木君在第1回合移动到坐标 $1$，在第2回合留在原地，因此将在2回合后找到高桥君。