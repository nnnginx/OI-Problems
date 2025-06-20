# AT_indeednow_2015_finala_e Page Rank

## 题目描述

在某家公司中，有 $ n $ 名员工。  
这些员工的座位排成一条直线，从一端开始依次分配编号。  
为了评估每位员工的能力，公司采用了以下方法。

每位员工都需提交一份他们认为优秀的同事名单。  
将第 $ i $ 位员工提交的名单记作 $ N(i) $。  
由于距离较远的员工们互相了解不多，因此 $ N(i) $ 之中不会包含与第 $ i $ 位员工相距超过 10 个座位的同事。  
（对于 $ x \in N(i) $，满足 $ |i - x| < 10$。）

收齐所有的名单后，公司构建出一个以员工为顶点、以“认为优秀”的关系为有向边的图。  
然后，利用该图计算每位员工的 Page Rank 值作为能力指标。  
定义第 $ i $ 位员工的 Page Rank 为 $ PR(i) $，而认为第 $ i $ 位员工优秀的员工集合为 $ M(i) $。Page Rank 满足如下公式：
$$
PR(i) = 0.1 + 0.9 \sum_{j \in M(i)} \frac{PR(j)}{|N(j)|}
$$

你的任务是为公司编写一个程序，求解每位员工的 Page Rank。

## 输入格式

输入内容如下：

> $ n $ $ m $  
> $ a_1 $ $ b_1 $  
> $\vdots$  
> $ a_m $ $ b_m $

- 第一行包含两个整数 $ n $ 和 $ m $，分别表示员工总数和“优秀”关系的数量（$ 1 \leq n \leq 10,000 $，$ 1 \leq m \leq 10,000 $）。
- 接下来的 $ m $ 行中，每行包含两个整数 $ a_i $ 和 $ b_i $，表示第 $ a_i $ 名员工认为第 $ b_i $ 名员工优秀（$ 1 \leq a_i, b_i \leq n $，且 $ |a_i - b_i| < 10 $）。

## 输出格式

输出每位员工的 Page Rank 值，每个值单独占一行。

如果相对误差或绝对误差不超过 $ 10^{-6} $，则结果被视为正确。

## 输入输出样例 #1

### 输入 #1

```
3 6
1 2
1 3
2 1
2 3
3 1
3 2
```

### 输出 #1

```
1
1
1
```

## 输入输出样例 #2

### 输入 #2

```
3 4
1 2
1 3
2 1
3 1
```

### 输出 #2

```
1.473684210526316
0.7631578947368423
0.7631578947368423
```

## 说明/提示

### 示例解释 2

在这个示例中，有 3 位员工。第 1 位员工认为第 2 和第 3 位员工都很优秀。第 2 位员工认为第 1 位员工优秀。第 3 位员工也认为第 1 位员工优秀。因此，各位员工的 Page Rank 应满足以下条件：
$$
PR(1) = 0.1 + 0.9 \left( \frac{PR(2)}{1} + \frac{PR(3)}{1} \right)
$$
$$
PR(2) = 0.1 + 0.9 \left( \frac{PR(1)}{2} \right)
$$
$$
PR(3) = 0.1 + 0.9 \left( \frac{PR(1)}{2} \right)
$$

 **本翻译由 AI 自动生成**