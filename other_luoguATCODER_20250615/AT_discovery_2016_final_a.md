# AT_discovery_2016_final_a DISCO presents ディスカバリーチャンネルプログラミングコンテスト 2016 Ⅱ

## 题目描述

有 $N$ 个人参加比赛，其中：

第一名可以获得 $100000$ 日元；

第二名可以获得 $50000$ 日元；

第三名可以获得 $30000$ 日元；

第四名可以获得 $20000$ 日元；

第五名可以获得 $10000$ 日元；

其余名次没有奖金。

要求按照参赛者编号 $id$ 依次输出每个人获得的奖金数量。

## 输入格式

第一行一个整数 $N(5\le N\le100)$，表示参赛者数量。

接下来有 $N$ 行，第 $i$ 行一个整数 $id_i(1\le id_i\le N)$，表示第 $i$ 名的参赛者编号是 $id_i$。

## 输出格式

输出 $N$ 行，第 $i$ 行表示参赛者编号为 $id_i$ 的选手获得的奖金数量。

## 输入输出样例 #1

### 输入 #1

```
5
1
2
3
4
5
```

### 输出 #1

```
100000
50000
30000
20000
10000
```

## 输入输出样例 #2

### 输入 #2

```
8
8
7
6
5
4
3
2
1
```

### 输出 #2

```
0
0
0
10000
20000
30000
50000
100000
```

## 输入输出样例 #3

### 输入 #3

```
7
1
5
4
2
7
6
3
```

### 输出 #3

```
100000
20000
0
30000
50000
0
10000
```