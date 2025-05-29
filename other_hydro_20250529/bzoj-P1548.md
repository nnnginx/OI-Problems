## 题目描述
A group of $n$ children are playing with a set of $n^2$ flat square blocks. Each block is painted from above with one colour, and there are no more than $2$ blocks of each colour. The blocks are initially arranged in an $n^2$ square forming some sort of picture.

The children have been provided with some other $n^2$ picture and asked to rearrange the blocks to that form. Since this is not really what they enjoy doing most, they intend to solve the task together and spend as little time on it as possible. Thus, every minute each child chooses a single $1 \times n$ row or $n \times 1$ column of blocks to rearrange. This row/column may never intersect with rows/columns chosen by other children in the same minute. A child takes one minute to perform any rearrangement (permutation) of the blocks within its row/column it likes.

Determine whether the children can perform their task of converting one block image into the other, and if so -- find the minimum possible time in minutes required to achieve this.

![](https://hydro.org.cn/d/bzoj/p/1548/file/pic1%20(8).jpg)

一群 $n$ 个孩子在玩一组 $n^2$ 个扁平方块。每个块都是用一种颜色绘制的，每种颜色最多只能存在于 $2$ 个块上。这些块最初排列在形成某种图片的 $n^2$ 正方形中。

现在给孩子们提供了一个大小为 $n^2$ 图片，并要求他们重新排列该表格的形式。由于这并不是他们最喜欢做的事情，因此，他们打算共同解决任务，并花最少的时间在任务上。因此，每个孩子每分钟都会选择一行或一列来重新排列。该行/列可能永远不会与同一时间其他孩子选择的行/列相交。孩子需要一分钟的时间对其喜欢的行/列中的块进行任何重新排列。

确定孩子们是否可以执行将一个块图像转换为另一个块图像的任务，如果可以，请找到达到此目的所需的最短时间（以分钟为单位）。 

Translated by wheneveright.

## 输入格式
第一行一个数 $t$，表示测试数据的组数。

每一组第一行一个数 $n$，表示棋盘的大小。

接下来 $n$ 行，每行 $n$ 个数，第 $i$ 行第 $j$ 列一个数 $a_{i,j}$ 表示初始棋盘中的每一个数。再接下来 $n$ 行，每行 $n$ 个数，第 $i$ 行第 $j$ 列一个数 $b_{i,j}$ 表示目标棋盘中的每一个数。

## 输出格式
对于每组数据，你都要输出一个最小的变换次数，若初始状态不能变换到目标状态则输出 `no`。

## 样例输入
```plain
10
3
5 5 6 
3 2 4 
7 2 1 
2 4 2 
5 1 6 
5 7 3 
3
3 3 5 
6 2 1 
1 6 9 
3 1 3 
5 6 1 
2 6 9 
3
7 8 3 
8 5 5 
3 4 1 
1 7 3 
8 8 4 
5 5 3 
3
4 2 6 
8 1 4 
8 1 3 
2 3 4 
4 6 8 
1 1 8 
3
2 7 1 
3 2 5 
8 8 9 
5 8 8 
1 9 2 
2 7 3 
3
7 8 3 
3 6 2 
2 1 6 
2 6 8 
1 2 6 
7 3 3 
3
2 8 3 
7 2 8 
6 5 4 
8 7 6 
5 2 4 
2 3 8 
3
1 6 8 
9 8 1 
3 3 5 
8 1 9 
8 6 1 
3 3 5 
3
7 9 4 
9 7 1 
2 2 4 
2 7 4 
1 9 4 
7 9 2 
3
6 2 2 
8 6 1 
7 3 5 
2 6 6 
7 2 3 
1 8 5 

```
## 样例输出
```plain
3
2
3
2
3
2
3
2
3
3
```

## 数据规模及约定

| 测试点 | t | n | 时限 |
| ----------- | ----------- | ----------- | ----------- |
| 1 | t=10 | n=3 | 1s |
| 2 | t=10 | n<=10 | 1s |
| 3 | t=50 | n<=10 | 1s |
| 4-5 | t=200 | n<=100 | 2s |
| 6-7 | t=200 | n<=200 | 7s |
| 8-10 | t=200 | n=200 | 15s |

其中所有数据保证 $a_{i,j},b_{i,j}\le n^2$。

## 题目来源
HNOI2009 集训 Day4