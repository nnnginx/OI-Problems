## 题目描述

农场面临着洪水的威胁。帮助约翰找到水的高度，他可以把他的奶牛移到安全的地方, 农场由 $m × n(1 ≤ m, n ≤ 400)$ 的单位方格组成．每格有一个海拔高度 $h_{i,j}(1≤h_{i,j}≤10000)$。给出一个 $m × n$ 的表格地图和降水量 $v$ (1≤ v ≤10^9)。水总是先注入最低的方格，不管该方格在哪儿。请你算出水面高度，水面和海平面之间的陆地体积（可能为 $0$）。注意：陆地和水面高度相同时已经被淹没。

## 输入格式

第 $1$ 行：有三个整数 $m, n, v$。

Lines 2...: Each line contains as many as 20 space-separated integers that represent the elevations of the farm. The first N integers are spread across line 1 and it successors, 20 integers per line, until all N integers are laid out. The next N integers begin on a new line, etc.

## 输出格式

在一行内输出两个由空格分隔的整数：水面高度，海平面和水面之间陆地的体积（被水完全淹没的陆地体积）。

```input1
4 5 33
2 2 2 2 2
1 3 4 3 2
2 3 5 3 2
2 4 1 1 2
```

```output1
4  43
```

## 提示

水高 $4$ 米，淹没的区域标记 $1, 2, 3, 4$ 。水下陆地的体积：$1 × 3 + 2 × 10 + 3 × 4 + 4 × 2 = 43$ 。

## 题目来源

Orange

