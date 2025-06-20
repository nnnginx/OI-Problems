# AT_abc024_c [ABC024C] 民族大移動

## 题目描述

### 题意简述
高桥君的王国有 $N$ 个城市，每个城市用编号 $1$ ~ $N$ 表示。

高桥国有 $K$ 个民族居住，第 $i$ 个民族生活在编号为 $S_i$ 的城市。

高桥国有百年一度的所有民族共同习俗**民族大迁徙**，但由于交通拥堵，所以设置了**第 $i$ 天只能在编号在 $L_i$ 到 $R_i$ 的城市来来去去**的限制，并最多花费 $D$ 天进行。

每个民族都遵守这一行动限制，在经过几个城市的同时前往目的地城市。

第 $i$ 个民族的目的地是 $T_i$ ，每个民族都希望尽可能早的到达目的地。

求每个民族最早到达目的地的时间。

## 输入格式

第一行有 $3$ 个整数，分别为高桥国城市的个数 $N$ ，大迁徙的时间 $D$，高桥国所住的民族数 $K$。

接下来的 $D$ 行，有 $2$ 个整数 $L_i,R_i$，表示第 $i$ 天可来来去去的城市编号范围。

接下来的 $K$ 行，每行 $2$ 个整数 $S_i,T_i$，表示第 $i$ 个民族原本居住的城市编号和目的地城市编号。

## 输出格式

共 $K$ 行，每行一个整数表示第 $i$ 个民族到达目的地的最少天数。

数据保证每个民族 $D$ 天内能到达目的地。

## 输入输出样例 #1

### 输入 #1

```
10 10 3
1 5
3 6
7 10
5 8
4 4
1 4
2 9
1 3
1 1
4 5
1 6
2 7
10 1
```

### 输出 #1

```
2
4
8
```

## 输入输出样例 #2

### 输入 #2

```
10 10 4
1 2
2 4
3 6
4 8
5 10
9 10
7 8
5 6
3 5
1 3
10 1
3 8
2 4
1 3
```

### 输出 #2

```
10
4
2
2
```

## 输入输出样例 #3

### 输入 #3

```
314159265 10 1
1 10000
500 12031
1414 113232
111111 777777
666661 23423423
12345678 123456789
111111111 314159265
112334 235235235
1 223445
314 1592
1 314159265
```

### 输出 #3

```
7
```