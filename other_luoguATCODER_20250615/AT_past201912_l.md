# AT_past201912_l グラデーション

## 题目描述

平面直角坐标系上有 $n$ 个**普通点**和 $m$ 个**特殊点**。第 $i$ 个**普通点**的坐标为 $(x_i,y_i)$，颜色为 $c_i$；第 $i$ 个**特殊点**的坐标为 $(p_i,q_i)$，颜色为 $o_i$。**同一个坐标上可能有多个点。**

你想用线段连接一些点，使得任意两个**普通点**之间都可以通过在线段上移动到达。画一条新线段的成本在线段两端点同色时为线段长度，异色时为线段长度的 $10$ 倍。（在此，我们不考虑相交的线段。）

输出达成目标的最小总成本。

## 输入格式

第一行输入两个整数 $n$ 和 $m$。

接下来 $n$ 行，每行三个整数 $x_i,y_i,c_i$。

接下来 $m$ 行，每行三个整数 $p_i,q_i,o_i$。

## 输出格式

输出一行一个实数，最小总成本。你的答案与标准答案的误差不超过 $10^{-6}$ 即可被判定为通过。

### 数据规模与约定

$2 \le n \le 30$，$1 \le m \le 5$，$0 \le x_i,y_i,p_i,q_i \le 1000$，$1 \le c_i,o_i \le 3$。（$1,2,3$ 分别表示红、绿、蓝三色）

## 输入输出样例 #1

### 输入 #1

```
3 1
0 0 1
0 1 1
1 0 1
1 1 1
```

### 输出 #1

```
2.000000000000
```

## 输入输出样例 #2

### 输入 #2

```
3 1
0 10 1
10 0 2
10 20 3
10 10 1
```

### 输出 #2

```
210.000000000000
```