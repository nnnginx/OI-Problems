## 题目描述

有 $2n$ 个士兵站成两排，他们需要被重新排列，以保证每一排里没有同样高的士兵——这样我们就说，士兵们被合理地安排了位置。 每次操作可以交换两个在同一位置（但不在同一排）的士兵。你的任务是用最少的操作来确保士兵们被合理地安排了位置。 例如： 有 $18$ 个士兵站成两排，箭头标明了重新安排士兵位置的正确方式（图飞了?）。 写一个这样的程序： 读入 $n$ 与士兵的身高，以及他们最初所站的位置，确保以最小的交换（站在同一位置的不同排的士兵）的次数来合理地安排士兵的位置，输出操作数。

## 输入格式

第一行为一个整数 $n$，接下来的两行每行有 $n$ 个数表示每行站着的 $n$ 个士兵的身高 $h_i$。 数据保证你能够合理地安排士兵的位置（即每个数在 $2n$ 个数中最多出现两次）。

## 输出格式

只有一行，输出最小操作数。

![](https://cdn.luogu.org/upload/pic/14829.png)

## 题目描述

$2n$ soldiers are standing in a double-row. They have to be rearranged, so that there are no equally tall soldiers in each row - then we shall say, that the soldiers are set up properly.

A single operation consists in swapping two soldiers who occupy the same position (but in different rows). Your task is to determine the minimum number of swaps necessary to set the soldiers up properly.

Example:

There is a double-row of $18$ soldiers in the figure. Arrows indicate the swaps that rearrange the soldiers in a proper way.

TaskWrite a programme that:

reads from the standard input the number and heights of soldiers, as they stand initially,determines the minimum number of swaps (of soldiers standing on the same position in different rows) necessary to set up soldiers properly,writes the result to the standard output.

**一句话题意：$2n$ 个数站成两排（每个数在 $2n$ 个数中最多出现两遍），一次操作可以交换任意一列中两个数，求使每行数不重复的最少操作数。**

## 输入格式

In the first line of the input there is one integer $n$, $1\le n\le 50\ 000$. In each of the two rows there are $n$ soldiers standing. In each of the following two lines there are $n$ positive integers separated by single spaces. In the second line there are numbers $x_1,x_2,\cdots,x_n$, $1\le x_i\le 100\ 000$; $x_i$ denotes the height of the $i$'th soldier in the first line. In the third line there are numbers $y_1,y_2,\cdots,y_n$, $1\le y_i\le 100\ 000$; $y_i$ denotes the height of the $i$'th soldier in the second line.

It is guaranteed that in the instances from the test data it is possible to set up soldiers properly.

## 输出格式
In the first and only line of the standard output one integer should be written - the minimum number of swaps necessary to set up soldiers properly.

## 输入样例
```plain
9
2 5 5 2 7 4 7 3 9
1 6 8 4 6 3 9 1 8
```


## 输出样例
```plain
3
```

## 数据规模及约定

对于 $100 \%$ 的数据：$1 \le n \le 5 \times 10^4$, $1 \le h_i \le 10^5$