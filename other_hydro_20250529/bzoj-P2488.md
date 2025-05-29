## 题目描述

John and Brus believe that number $N$ is a very bad number．Thus they try to avoid it every time and everywhere．  
Now the guys would like to represent number $M$ as a sum of positive numbers，each of which not exceeding $K$．But don’t forget about the bad number $N$！Each summand must not be divisible by $N$，moreover the number of summands also must not be divisible by $N$．  
Your task is to find the minimal possible number of summands in such representation of $M$．  
For example，if $N=3,M=11,K=6$ then we can represent $M$ as $5+6$，but as far as $6$ is divisible by $3$ we must have at least $3$ summands．But as far as $N=3$ we can’t have $3$ summands and thus the answer is $4$．One of the possible ways to represent $M$ is $11=4+4+2+1$．

给你三个整数 $N,M,K$，求一个最小的 $P$，使得 $M$ 能够被分成 $P$ 个正整数的和。  
并且这些整数要满足：（一）不能是 $N$ 的倍数，（二）大小不能超过 $K$，并且 $P$也不能是 $N$ 的倍数。

## 输入格式

The first line contains single integer $T$ – the number of test cases．Each test case consists of a single line containing three integers $N,M$ and $K$ separated by single spaces．

## 输出格式
 
For each test case print a single line containing the minimal possible number of summands according to the requirements described above．If it is impossible to do this output `-1` （quotes for clarity） instead．

```input1
2
3 11 6
2 12 47
```

```output1
4
-1
```

## 数据规模与约定

$100\%$ 的数据满足：$1 \le T \le 74,N,M,K \le 10^9$。