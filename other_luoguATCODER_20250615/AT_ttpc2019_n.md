# AT_ttpc2019_n 瓜二つ

## 题目描述

双胞胎 **尤里（Yuri）** 和 **穆里（Muri）** 虽然长得一模一样，但性格完全相反。例如，尤里喜欢**有理数**，而穆里则喜欢**无理数**。  
他们将用 $N$ 个杯子进行以下游戏：

- 最开始，第 $i$ 个杯子中有 $W_i$ 升水，同时定义两个数 $l_i, u_i$，其中 $l_i < u_i$。
- 他们**轮流**进行操作，**无法进行操作的一方输掉游戏**。

游戏的操作规则如下：

1. 选择一个整数 $k$ ($1 \leq k \leq N$)，并记该杯中剩余的水量为 $R_k$ 升。
2. 选择一个满足 $l_k \leq x \leq u_k$ 且 $x \leq R_k$ 的数 $x$，然后从该杯中喝掉 $x$ 升的水。  
   - **尤里（Yuri）**只能选择**有理数** $x$。
   - **穆里（Muri）**只能选择**无理数** $x$。  
   - 如果找不到符合条件的 $x$ 和 $k$，则无法进行操作，当前玩家输掉游戏。

由于输入中所有的 $W_i, l_i, u_i$ 都是整数，为了保证游戏可行，**穆里（Muri）可以决定自己是否先手**。

假设双方都采取最优策略，请判断谁能获胜：

- 如果尤里（Yuri）获胜，则输出 `"Yuri"`。
- 如果穆里（Muri）获胜，则输出 `"Muri"`。

## 输入格式

从标准输入读取以下格式的数据：

```
N
W_1 l_1 u_1
W_2 l_2 u_2
...
W_N l_N u_N
```

## 输出格式

如果尤里（Yuri）获胜，输出 `"Yuri"`；如果穆里（Muri）获胜，输出 `"Muri"`。

## 输入输出样例 #1

### 输入 #1

```
2
8 2 5
7 5 6
```

### 输出 #1

```
Muri
```

## 输入输出样例 #2

### 输入 #2

```
1
1 1 2
```

### 输出 #2

```
Yuri
```

## 输入输出样例 #3

### 输入 #3

```
5
12 1 100
11 2 8
1 5 7
7 5 7
29 4 5
```

### 输出 #3

```
Muri
```

## 说明/提示

### 限制

- 所有输入均为整数
- $1 \le N \le 2 \times 10^5$
- $1 \le W_i \le 10^9$
- $1 \le l_i < u_i \le 10^9$

### 样例解释 1

- 穆里选择**先手**，并在第一个杯子里选 $x = 5 - \pi / 4$，此时第一个杯子剩余 $3 + \pi / 4$ 升水。
- 尤里只能选择有理数，他选择 $x = 2$，导致剩余 $1 + \pi / 4$。
- 之后穆里可以在第二个杯子执行类似操作，最终导致尤里无路可走，穆里获胜。

### 样例解释 2

- 只有 $1 \leq x \leq 2$ 且 $x \leq 1$，唯一满足条件的 $x = 1$ 是整数，因此尤里可以选择它。
- 由于整数也是有理数，尤里可以执行该操作，而穆里无法选取无理数，所以穆里无法行动，尤里获胜。