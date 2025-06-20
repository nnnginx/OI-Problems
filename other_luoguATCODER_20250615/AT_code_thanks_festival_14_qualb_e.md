# AT_code_thanks_festival_14_qualb_e マスゲーム

## 题目描述

有一个大小为 $R \times C$ 的二维网格，左上角的格子坐标为 $(1,1)$，右下角的坐标为 $(R,C)$。

你需要在这个网格上执行 $N$ 次操作，每次操作将某个矩形区域内所有的格子涂成黑色。具体操作为：给定四个整数 $r, c, h, w$，表示起始坐标为 $(r,c)$，并在此基础上构建一个纵向长度为 $h$、横向长度为 $w$ 的矩形区域，将该区域内的 $h \times w$ 个格子全部涂黑。

你现在位于网格上的一个位置，希望只通过黑色的格子走到另一个位置。移动时，可以选择上下左右相邻的格子，但不能移出网格的边界。

给定起点坐标 $(r_s, c_s)$ 和终点坐标 $(r_g, c_g)$ 以及若干次涂色操作，问你是否能够只通过黑色格子从起点走到终点。如果可以，输出 `YES`；否则，输出 `NO`。注意，起点和终点必须都是黑色的。

## 输入格式

输入从标准输入中给出，格式如下：

- 第一行包含两个整数 $R$ 和 $C$，表示网格的行数和列数，满足 $1 \leq R, C \leq 48$。
- 第二行包含两个整数 $r_s$ 和 $c_s$，表示起点的坐标，满足 $1 \leq r_s \leq R$，$1 \leq c_s \leq C$。
- 第三行包含两个整数 $r_g$ 和 $c_g$，表示终点的坐标，满足 $1 \leq r_g \leq R$，$1 \leq c_g \leq C$。
- 第四行包含一个整数 $N$，表示操作的次数，满足 $1 \leq N \leq 1000$。
- 接下来的 $N$ 行，每行包含四个整数 $r_i, c_i, h_i, w_i$，表示第 $i$ 个矩形的左上角坐标 $(r_i, c_i)$ 以及它的纵向长度 $h_i$ 和横向长度 $w_i$。这些整数满足 $1 \leq r_i \leq R$，$1 \leq c_i \leq C$，$1 \leq r_i + h_i - 1 \leq R$，$1 \leq c_i + w_i - 1 \leq C$。
- 保证起点和终点必定不同，即 $(r_s, c_s) \neq (r_g, c_g)$。

## 输出格式

输出 `YES` 或 `NO` 来表示是否能从起点通过黑色格子到达终点。请在最后输出换行符。

### 示例解释

假设白色格子用 `.` 表示，黑色格子用 `#` 表示，在进行涂色操作后，网格可能呈现如下：
```plaintext
.....
.####
...#.
...#.
```

起点用 `S` 表示，终点用 `G` 表示，则他们在网格中的位置可能是这样的：
```plaintext
.....
.S...
...G.
.....
```

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
4 5
2 2
3 5
2
2 2 1 4
3 5 2 1
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
4 5
1 2
2 2
2
1 1 1 5
1 1 4 1
```

### 输出 #2

```
NO
```

## 输入输出样例 #3

### 输入 #3

```
4 5
1 1
1 3
3
1 1 1 1
1 2 1 1
1 3 1 1
```

### 输出 #3

```
YES
```

## 输入输出样例 #4

### 输入 #4

```
1 5
1 1
1 2
1
1 3 1 2
```

### 输出 #4

```
NO
```

## 输入输出样例 #5

### 输入 #5

```
1 5
1 3
1 2
1
1 3 1 2
```

### 输出 #5

```
NO
```

## 输入输出样例 #6

### 输入 #6

```
48 48
1 1
48 48
1
1 1 48 48
```

### 输出 #6

```
YES
```