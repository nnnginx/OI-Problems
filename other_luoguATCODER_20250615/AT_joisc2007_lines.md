# AT_joisc2007_lines 直線 (Lines)

## 题目描述

平面上有 $N$ 条直线 $l_1,l_2,...,l_N$。$l_i$ 经过坐标系上的点 $P_i(a_i,b_i)$ 和 $Q_i(c_i,d_i)$。请问：这 $N$ 条直线将平面分成了几个部分？

## 输入格式

第一行为一个整数 $N$。

接下来 $N$ 行，第 $i$ 行为四个整数 $a_i,b_i,c_i,d_i$。

## 输出格式

一行一个整数，区域个数。

### 输入输出样例

#### 输入 #1

```
4
0 4 6 4
0 0 6 6
1 0 1 6
0 6 6 0
```

#### 输出 #1

```
11
```

#### 数据规模与约定

对于全部测试点，数据保证 $1\le N\le 1000$，$0\le a_i,b_i,c_i,d_i\le 1000$，$(a_i,b_i)\neq(c_i,d_i)$。