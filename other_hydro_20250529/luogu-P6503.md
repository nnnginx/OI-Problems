## 题目描述
给出一个长度为 $n$ 的序列 $a_i$，求出下列式子的值：

$$\sum_{i=1}^{n} \sum_{j=i}^{n} (\max_{i\le k\le j} a_k-\min_{i\le k\le j} a_k)$$



即定义一个子序列的权值为序列内最大值与最小值的差。求出所有连续子序列的权值和。



## 输入格式
输入第一行一个整数 $n$，表示序列的长度。

接下来的 $n$ 行，每行一个整数 $a_i$，描述这个序列。

## 输出格式
输出一行一个整数，表示式子的答案。

```input1
3
1
2
3
```

```output1
4
```

```input2
4
7
5
7
5
```

```output2
12
```

```input3
4
3
1
7
2
```

```output3
31
```

## 提示
#### 数据规模与约定

对于 $100\%$ 的数据，保证 $2\le n\le 3\times 10^5$，$1\le a_i\le 10^8$。

#### 说明

**题目译自 [COCI2010-2011](https://hsin.hr/coci/archive/2010_2011/) [CONTEST #3](https://hsin.hr/coci/archive/2010_2011/contest3_tasks.pdf) *T5 DIFERENCIJA***。

