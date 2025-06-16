## 题目描述
In what seems to be a familiar occurrence, Farmer John is lining up his $N$ cows $(1\le N\le 10^5)$, conveniently numbered $1\cdots N$, for a photograph.
Initially, the cows are lined up in the order $a_1,a_2,\cdots ,a_N$ from left to right. Farmer John's goal is to line up the cows in the order $b_1,\cdots ,b_N$ from left to right. To accomplish this, he may perform a series of modifications to the ordering. Each modification consists of choosing a single cow and moving it some number of positions to the left.

Please count the minimum number of modifications required in order for Farmer John to line up his cows in the desired order.

## 输入格式
The first line of input contains $N$. The second line contains $a_1,a_2,\cdots ,a_N$. The third line contains $b_1,\cdots ,b_N$.

## 输出格式
Print the minimum number of modifications required to produce Farmer John's desired ordering.

## 题目大意
### 题目描述

在一个熟悉的情景中，Farmer John 正在为他的 $N$ 头奶牛（$1 \leq N \leq 10^5$，编号为 $1 \cdots N$）排队拍照。  
初始时，奶牛从左到右的排列顺序为 $a_1, a_2, \cdots , a_N$。Farmer John 的目标是将奶牛从左到右排列成 $b_1, \cdots , b_N$ 的顺序。为了实现这一目标，他可以对排列顺序进行一系列修改。每次修改包括选择一头奶牛并将其向左移动若干位置。

请计算 Farmer John 将奶牛排列成目标顺序所需的最少修改次数。

### 输入格式

输入的第一行包含 $N$。第二行包含 $a_1, a_2, \cdots , a_N$。第三行包含 $b_1, \cdots , b_N$。

### 输出格式

输出将奶牛排列成目标顺序所需的最少修改次数。

### 样例解释 1

在这个例子中，奶牛已经处于目标顺序，因此不需要任何修改。

### 样例解释 2

在这个例子中，两次修改即可满足要求。以下是 Farmer John 重新排列奶牛的一种方式：

- 选择奶牛 $4$ 并将其向左移动四个位置。
- 选择奶牛 $2$ 并将其向左移动两个位置。
```
   5 1 3 2 4
-> 4 5 1 3 2
-> 4 5 2 1 3
```

### 数据范围

- 测试用例 3-6 满足 $N \leq 100$。
- 测试用例 7-10 满足 $N \leq 5000$。
- 测试用例 11-14 没有额外限制。

```input1
5
1 2 3 4 5
1 2 3 4 5
```

```output1
0
```

```input2
5
5 1 3 2 4
4 5 2 1 3
```

```output2
2
```

## 提示
【样例解释 1】

In this example, the cows are already in the desired order, so no modifications are required.

【样例解释 2】

In this example, two modifications suffice. Here is one way Farmer John can rearrange his cows:

- Choose cow $4$ and move it four positions to the left.
- Choose cow $2$ and move it two positions to the left.
```
   5 1 3 2 4
-> 4 5 1 3 2
-> 4 5 2 1 3
```

【数据范围】

- Test cases 3-6 satisfy $N≤100$.
- Test cases 7-10 satisfy $N≤5000$.
- Test cases 11-14 satisfy no additional constraints.

