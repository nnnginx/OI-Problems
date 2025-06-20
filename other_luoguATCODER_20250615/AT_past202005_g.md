# AT_past202005_g グリッド金移動

## 题目描述

在平面直角坐标系上有一枚棋子，最初它被放置在坐标系的原点处。

在坐标系中，还有许多干扰棋子。这样的棋子一共有 $n$ 枚，第 $i$ 枚棋子被放置在 $(x_i,y_i)$ 处。在移动时，不可以经过这些点。

当你移动的棋子在 $(x,y)$ 处时，你在下一步可以移动到以下几个点之一：

- $(x+1,y+1)$
- $(x,y+1)$
- $(x-1,y+1)$
- $(x+1,y)$
- $(x-1,y)$
- $(x,y-1)$

请求出将这枚棋子移动到 $(r,c)$ 所需的最少步数。若无法到达，请输出 $-1$。

## 输入格式

第一行输入三个正整数 $n,r,c$。

接下来 $n$ 行，每行输入两个数 $x_i,y_i$，表示每个干扰棋子的坐标。

## 输出格式

一行一个整数，答案。

## 输入输出样例 #1

### 输入 #1

```
1 2 2
1 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
1 2 2
2 1
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
5 -2 3
1 1
-1 1
0 1
-2 1
-3 1
```

### 输出 #3

```
6
```

## 说明/提示

#### 数据规模与约定

对于所有测试点，数据保证 $1 \le n \le 800$，$|x_i|,|y_i|,|r|,|c| \le 200$，没有两个及两个以上的干扰棋子在同一位置，起点和终点上均无干扰棋子，且起终点位置不同。

保证所有输入数据均为整数。