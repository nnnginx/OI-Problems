## 题目描述


You are given a list of $n$ integers $a_{1},$ . . . , $a_{n}.$ You can perform the following operation: choose some $a_{i}$ and multiply it by any positive integer.

Your task is to compute the minimum number of different integers that could be on the list after $k$ operations for all $0 \le k \le n$ .



## 输入格式


The first line of the input contains single integer $n (1 \le n \le 3·10^{5}).$ The second line of the input contains $n$ integers $a_{i} (1 \le a_{i} \le 10^{6}).$



## 输出格式


Output a single line that contains $n + 1$ integers. The i-th integer should be the minimum possible number of different integers in the list after $i − 1$ operations.



## 题目大意
给定一个长度为 $n$ 的数列 $a_1,a_2,a_3,...,a_n$，每次操作，你可以让某个被选定的数乘上任意一个正整数。

现在。对于所有的 $k\in[0,n]$，求出经过 $k$ 次操作后数列里面不同的数的数量能够达到的最小值。

Translated by Eason_AC  
2020.11.15

```input1
6
3 4 1 2 1 2

```

```output1
4 4 3 3 2 2 1

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



