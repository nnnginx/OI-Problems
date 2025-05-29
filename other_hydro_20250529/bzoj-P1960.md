## 题目描述

There is a large number of empty bins in a factory depot. The bins are arranged in a single row. The manager of the depot wants to put some bins into other bins to make some free space in the left end of the depot. Bins can be moved by a robot, which can take a bin, carry it to the right, and put it into a larger bin. This three-operation sequence is the only allowed way to move bins.

Because of safety regulations, any bin can contain at most one other bin, which must be empty. The manager also wants to keep the double bins in the left end of the resulting row, to make it easier to keep track of them.

You are to write a program that computes the largest possible $k$ such that the $k$ leftmost bins can be put into the immediately following $k$ bins in some order.

## 输入格式

The first line of the text file `bins.in` contains two integers, separated by a space: $m$, the size of the largest bin, and $n$, the number of bins. The second line contains $n$ integers $a_i(1 \le a_i \le m)$, separated by spaces: the sizes of the bins, listed from left to right.

## 输出格式

The first and only line of the text file `bins.out` should contain a single integer, the
largest number $k$ such that the robot can put the $k$ leftmost bins into the next $k$ bins.

```input1
5 10
2 2 1 4 3 2 5 4 2 3
```
```output1
4
```

## 数据规模与约定

For all the test cases, $1 \le n \le 2 \times 10^4$, $1 \le m \le 10^3$.

