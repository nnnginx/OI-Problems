# AT_joisc2007_mall ショッピングモール (Mall)

## 题目描述

### 题目简述

有一个 $n\times m$ 的网格 $c$，你需要在其中选择一个 $b\times a$ 的长方形（不可旋转），使得它满足：

- 长方形内任何一个格子里的数非负；
- 长方形内所有格子的数之和最小。

求出和的最小值。

## 输入格式

第一行输入两个整数 $m,n$。

第二行输入两个整数 $a,b$。

第三行到第 $(n+2)$ 行，第 $(i+2)$ 行输入 $m$ 个整数，依次表示 $c_{i,1},c_{i,2},...,c_{i,m}$。

保证至少有一个满足条件的长方形。

## 输出格式

一行一个整数，表示最小和。**请在输出末尾换行。**

### 输入输出样例

```
7 6 
3 2
26 29 84 15 -1 1 71
45 14 38 91 62 77 35
68 -1 -1 90 63 56 70
31 2 4 74 72 41 90
100 26 21 -1 44 72 60
71 4 40 93 48 -1 50
```

```
184
```

## 说明/提示

#### 样例 #1 解释

$31+2+4+100+26+21=184$。

### 数据规模与约定

$1\le m,n\le 1000$，$1\le a,b\le 1000$，$-1\le c_{i,j}\le 100$。