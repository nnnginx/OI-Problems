## 题目描述
Farmer John has hired a professional photographer to take a picture of some of his cows.  Since FJ's cows represent a variety of different breeds, he would like the photo to contain at least one cow from each distinct breed present in his herd.

FJ's N cows are all standing at various positions along a line, each described by an integer position (i.e., its x coordinate) as well as an integer breed ID.  FJ plans to take a photograph of a contiguous range of cows along the line.  The cost of this photograph is equal its size -- that is, the difference between the maximum and minimum x coordinates of the cows in the range of the photograph.

Please help FJ by computing the minimum cost of a photograph in which there is at least one cow of each distinct breed appearing in FJ's herd.


## 输入格式
\* Line 1: The number of cows, N (1 <= N <= 50,000). 

\* Lines 2..1+N: Each line contains two space-separated positive integers specifying the x coordinate and breed ID of a single cow.  Both numbers are at most 1 billion.


## 输出格式
\* Line 1: The smallest cost of a photograph containing each distinct breed ID.


## 题目大意
### 问题描述

农民约翰雇一个专业摄影师给他的部分牛拍照。由于约翰的牛有好多品种，他喜欢他的照片包含每个品种的至少一头牛。

约翰的牛都站在一条沿线的不同地方， 每一头牛由一个整数位置 $X_i$ 以及整数品种编号 $ID_i$ 表示。

约翰想拍一张照片，这照片由沿线的奶牛的连续范围组成。照片的成本与规模相当，这就意味着，在一系列照片中的最大和最小 $X$ 坐标的差距决定了照片的成本。

请帮助约翰计算最小的照片成本，这些照片中有每个不同的品种的至少一头牛，没有两头牛愿意站在同一个地点的。


### 输入格式 


第 $1$ 行：牛的数量 $N$；


第 $2..1+N$ 行：每行包含 2 个以空格分隔的正整数 $X_i$ 和 $ID_i$；意义如题目描述；


### 输出格式 


输出共一行，包含每个不同品种 $\rm ID$ 的照片的最低成本。

```input1
6 
25 7 
26 1 
15 1 
22 3 
20 1 
30 1 

```

```output1
4 

```

## 提示
There are 6 cows, at positions 25,26,15,22,20,30, with respective breed IDs 7,1,1,3,1,1.


The range from x=22 up through x=26 (of total size 4) contains each of the distinct breed IDs 1, 3, and 7 represented in FJ's herd.


