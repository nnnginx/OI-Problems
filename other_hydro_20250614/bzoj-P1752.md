## 题目描述

Bessie is out in the field and wants to get back to the barn to get as much sleep as possible before Farmer John wakes her for the morning milking. Bessie needs her beauty sleep, so she wants to get back as quickly as possible.

Farmer John's field has $N$ landmarks in it, uniquely numbered $1\cdots N$. Landmark $1$ is the barn; the apple tree grove in which Bessie stands all day is landmark $N$. Cows travel in the field using $T$ bidirectional cow-trails of various lengths between the landmarks.

Bessie is not confident of her navigation ability, so she always stays on a trail from its start to its end once she starts it.

Given the trails between the landmarks, determine the minimum distance Bessie must walk to get back to the barn. It is guaranteed that some such route exists.

## 输入格式

* Line $1$: Two integers: $T$ and $N$.
* Lines $2\sim T+1$: Each line describes a trail as three space-separated integers. The first two integers are the landmarks between which the trail travels. The third integer is the length of the trail.

## 输出格式

* Line $1$: A single integer, the minimum distance that Bessie must travel to get from landmark $N$ to landmark $1$.

```input1
5 5
1 2 20
2 3 30
3 4 20
4 5 20
1 5 100
```

```output1
90
```

## 样例说明 

There are five landmarks. Bessie can get home by following trails $4$, $3$, $2$, and $1$.

## 数据规模与约定

对于 $100\%$ 的数据：$2 \leq N \leq 10^3$，$1 \leq T \leq 2*10^3$，$1\leq$ 铁轨长度 $\leq 100$。

## 题目来源

Usaco2005 qua