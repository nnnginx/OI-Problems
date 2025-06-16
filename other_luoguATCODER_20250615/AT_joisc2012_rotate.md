# AT_joisc2012_rotate 回転

## 题目描述

有一个 $N$ 行 $N$ 列的字符矩阵，定义第 $i$ 行第 $j$ 列的字符坐标为 $(i,j)$（$i,j$ 从 $1$ 开始）。

还有 $Q$ 次操作，第 $k$ 次操作将一个以 $(I_k,J_k)$ 为左上角的 $S_k\times S_k$ 大小的子矩阵逆时针旋转 $90$ 度。

你需要求出最终的矩阵。


接下来 $N$ 行，每行 $N$ 个字符，代表初始的字符矩阵。

## 输入格式

从标准输入读入数据。

## 输出格式

从标准输出输出数据。

$N$ 行，每行 $N$ 个字符，代表最终的字符矩阵。

### 输入输出样例

#### 输入 #1

```plains
4 1
abcd
efgh
ijkl
mnop
2 2 2
```

#### 输出 #1

```plains
abcd
egkh
ifjl
mnop
```

## 说明/提示

对于 $10\%$ 的数据，保证 $N \le 100,Q \le 100$。

对于 $100\%$ 的数据，保证 $2 \le N \le 1000,1\le Q \le 2000,2\le S_k \le N,1\le I_k\le N-S_k+1,1\le J_k\le N-S_k+1$。

#### 样例解释

初始方阵如下：

```plains
abcd
efgh
ijkl
mnop
```

第一次操作，选择以 $(2,2)$ 为左上角的 $2\times 2$ 的大小的子矩阵：

```plains
fg
jk
```

逆时针旋转 $90$ 度：

```plains
gk
fj
```

得到最终的矩阵：

```plains
abcd
egkh
ifjl
mnop
```