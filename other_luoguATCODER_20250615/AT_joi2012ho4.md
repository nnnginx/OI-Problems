# AT_joi2012ho4 釘 (Nails)

## 题目描述

板子上有 $n$ 行钉子，上起第 $i$ 行钉子有 $i$ 根。所有钉子排列成了一个正三角形。为表述简便，用 $(a,b)$ 表示上起第 $a$ 行的左起第 $b$ 根钉子（$1 \le a \le n$，$1 \le b \le a$）。

将“各边都平行于大三角形中的某一条，且方向与大三角形相同”的三角形定义为“好的三角形”。即，“好的三角形”的三个顶点的坐标分别为 $(a,b)$，$(a+x,b)$ 和 $(a+x,b+x)$。（$a,b$ 限制同上，$1 \le x \le n-a$）

给出钉子的行数 $n$、你拥有的橡皮筋根数 $m$ 和你套橡皮筋的方案，请求出：套完全部橡皮筋后，有多少根钉子被至少一根橡皮筋套住了？

## 输入格式

第一行两个正整数 $n,m$；

第二行到第 $(m+1)$ 行：每行三个正整数 $a_i,b_i,x_i$，表示将以 $(a_i,b_i)$，$(a_i+x_i,b_i)$ 和 $(a_i+x_i,b_i+x_i)$ 为顶点的三角形用橡皮筋围起来。

## 输出格式

一行一个整数，被至少一根橡皮筋围起来的钉子根数。

### 输入输出样例

#### 输入 #1

```
5 2
2 2 1
2 1 3
```

#### 输出 #1

```
12
```

## 说明/提示

#### 样例 #1 解释

除 $(1,1)$，$(4,4)$ 和 $(5,5)$ 外，其余的钉子均被围了起来。

#### 数据规模与约定

- $2 \le n \le 5000$，$1 \le m \le 500000$；