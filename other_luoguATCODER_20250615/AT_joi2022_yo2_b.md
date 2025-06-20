# AT_joi2022_yo2_b カーペット (Carpet)

## 题目描述

给出一个 $h \times w$ 的网格图。现在你在网格图中的 $(1,1)$ 处。你每次可以选择一个与你目前所在的格子上下左右相邻且颜色不同的格子并移动到上面。请求出到达 $(h,w)$ 的最少所需步数。若无法到达，请输出 $-1$。

## 输入格式

第一行：两个正整数 $h,w$。

接下来 $h$ 行：每行 $w$ 个字符，描述这个网格图。用`.`表示白色，`#`表示黑色。$(1,1)$ 在左上方。

## 输出格式

输出一行一个整数，答案。

## 输入输出样例 #1

### 输入 #1

```
4 5
...#.
#####
...#.
#.###
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
3 3
...
...
...
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
1 5
.#.#.
```

### 输出 #3

```
4
```

## 输入输出样例 #4

### 输入 #4

```
5 5
###.#
.#...
.#..#
.####
##..#
```

### 输出 #4

```
12
```

## 输入输出样例 #5

### 输入 #5

```
7 5
.#.##
##...
.#.##
.###.
##.#.
...#.
##.#.
```

### 输出 #5

```
12
```

## 说明/提示

#### 样例 #1 说明

其中一条最短路径为`(1,1)->(1,2)->(1,3)->(1,4)->(2,4)->(3,4)->(3,3)->(4,3)->(5,3)->(5,4)`。路径最短长度为 $9$。

#### 数据规模与约定

对于全部测试点，$1 \le h,w \le 500$，$(1,1) \neq (h,w)$，且 $h,w$ 均为整数。