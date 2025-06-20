# AT_abc320_e [ABC320E] Somen Nagashi

## 题目描述

现有 $N$ 个人排成一队，编号从 $1$ 到 $N$，玩一个叫做“流水面条”的游戏，该游戏共有 $M$ 个事件，每个事件含三个变量 $T_i,W_i,S_i$，事件的规则如下：

- 在 $T_i$ 时刻，有 $W_i$ 根面条流了下来，队头的人拿走这些面条，并离开队列，然后于第 $T_i+S_i$ 时刻返回队列，然后返回他的原始位置。

若队列为空，则该事件忽略。

注意：若他于第 $X$ 时刻返回队列，则视为他第 $X$ 时刻在队列。

一开始每个人都有 $0$ 根面条，现要你求出这 $N$ 个人每个人获得了多少面条。

## 输入格式

共 $M+1$ 行。

第 $1$ 行，共两个正整数，分别代表 $N,M$。

第 $2\sim M+1$ 行，第 $i+1$ 行三个正整数，分别代表 $T_i,W_i,S_i$。

## 输出格式

共 $N$ 行，第 $i$ 行代表第 $i$ 个人获得的面条。

## 输入输出样例 #1

### 输入 #1

```
3 5
1 1 3
2 10 100
4 100 10000
10 1000 1000000000
100 1000000000 1
```

### 输出 #1

```
101
10
1000
```

## 输入输出样例 #2

### 输入 #2

```
3 1
1 1 1
```

### 输出 #2

```
1
0
0
```

## 输入输出样例 #3

### 输入 #3

```
1 8
1 1 1
2 2 2
3 3 3
4 4 4
5 5 5
6 6 6
7 7 7
8 8 8
```

### 输出 #3

```
15
```

## 说明/提示

#### 样例#1说明：
第 $1$ 个人于 $1$ 时刻拿走 $1$ 根面条，将于 $4$ 时刻返回队列。

第 $2$ 个人于 $2$ 时刻拿走 $10$ 根面条，将于 $102$ 时刻返回队列。

第 $1$ 个人于 $4$ 时刻归队，返回第 $1$ 位，此时他处于队头，然后拿走 $100$ 根面条，将于 $10004$ 时刻返回队列。

第 $3$ 个人于 $10$ 时刻拿走 $1000$ 根面条，将于第 $1000000010$ 时刻归队。

第 $100$ 时刻，队内无人。

最终，这 $3$ 个人分别有 $101,10,1000$ 根面条。