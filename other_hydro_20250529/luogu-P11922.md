## 题目背景
PA 2025 R4C.



## 题目描述

有 $n$ 块正方体积木，编号 $1\sim a_i$。第 $i$ 块积木的边长为 $a_i$，图案种类为 $w_i$。

我们称一座**塔**是一个序列 $p_1,p_2,\ldots,p_m$，其中 $1\le p_i\le n$，且 $p_i$ 两两不同。

一座塔是**稳的**，当且仅当：

- $\forall 1\le i\lt m$，$a_{p_i}\gt a_{p_{i+1}}$。

给定正整数 $c$。定义一座塔的**美观度**为：

$$\sum_{1\le i\le m} a_{p_i}-c\cdot \sum_{1\le i\lt m} [w_{p_i}\neq w_{p_{i+1}}]$$

换句话说，是组成塔的积木高度减去（相邻的不同图案的积木对数乘以 $c$）。

求出**稳的**塔的最大美观度。


## 输入格式
第一行，正整数 $n,c$。

接下来 $n$ 行，第 $i$ 行两个正整数 $a_i,w_i$。

保证 $\forall 1\le i\lt n$，有 $a_i\le a_{i+1}$。


## 输出格式
输出一行一个整数，表示稳的塔的最大美观度。


```input1
4 1
1 1
3 2
4 3
4 1
```

```output1
6
```

```input2
4 5
1 1
3 2
4 3
4 1
```

```output2
5
```

## 提示
### 样例解释

**两个样例中**，四块积木的形状和图案如下所示。两个样例唯一的区别只有 $c$。

![](https://cdn.luogu.com.cn/upload/image_hosting/fgnbuet8.png?x-oss-process=image/resize,m_lfit,h_150)


样例 $1$ 中，下图的两个稳的塔的美观度是最大的，为 $4+3+1-(1+1)\times 1=6$。

![](https://cdn.luogu.com.cn/upload/image_hosting/ys9t7rao.png?x-oss-process=image/resize,m_lfit,h_150)


但是在样例 $2$ 中，上图的塔的美观度为 $-2$。样例 $2$ 中美观度最大的稳的塔如下所示，它的美观度为 $4+1-5\times 0=5$。

![](https://cdn.luogu.com.cn/upload/image_hosting/l1ou8e1y.png?x-oss-process=image/resize,m_lfit,h_100)

### 子任务

在价值 $50$ 分的子任务中，满足 $\forall 1\le i\lt n$，$a_i\lt a_{i+1}$。

### 数据范围

- $1\le n,c,a_i,w_i\le 5\times 10^5$；
- $\forall 1\le i\lt n$，$a_i\le a_{i+1}$。


