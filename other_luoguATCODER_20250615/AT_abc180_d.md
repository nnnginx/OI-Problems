# AT_abc180_d [ABC180D] Takahashi Unevolved

## 题目描述

Iroha 正在玩一个宠物养成的游戏。

Iroha 的宠物名字叫 Takahashi。初始，Takahashi 的 **STR** 值为 $X$，**EXP** 值为 $0$。Iroha 可以带宠物到以下任意一个 Gym 进行训练：

- Kakomon Gym：**STR** 值将会变为原来的 $A$ 倍，**EXP** 值将会加上 $1$。
- AtCoder Gym：**STR** 值将会加上 $B$，**EXP** 值将会加上 $1$。

当 Takahashi 的 **STR** 值大于等于 $Y$，Takahashi 会进化形态。

但是 Iroha 认为进化的 Takahashi 没那么可爱，于是 Iroha 想求出在保证 Takahashi 不进化的情况下，能达到的最大 **EXP** 值是多少。

## 输入格式

一行四个整数，$X\ Y\ A\ B$。

## 输出格式

一行一个表示最大 **EXP** 值的整数。

@[hellolin](/user/751017) 译

## 输入输出样例 #1

### 输入 #1

```
4 20 2 10
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
1 1000000000000000000 10 1000000000
```

### 输出 #2

```
1000000007
```