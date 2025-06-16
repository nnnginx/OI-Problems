## 题目描述
We are given a sequence of n decimal digits. The sequence needs to be partitioned into one or more contiguous subsequences such that each subsequence, when interpreted as a decimal number, is divisible by a given integer m. 

Find the number of different such partitions modulo $10^9 +7$. When determining if two partitions are different, we only consider the locations of subsequence boundaries rather than the digits themselves, e.g. partitions $2|22$ and $22|2$ are considered different.

## 输入格式
The ﬁrst line contains two integers n and m (1≤n≤300000, 1≤m≤1000000) – the length of the sequence and the divisor respectively. The second line contains a string consisting of exactly n digits.

## 输出格式
Output a single integer – the number of different partitions modulo 109 +7.

## 题目大意
有一个N位的数字，将其分割，保证每个区间里的数字可以被M整除

第一行输入N M

第二行输入待划分的数字

输出有多少种方法，对10^9+7取余

Translated by @chen_zhe

```input1
4 2
1246
```

```output1
4
```

```input2
4 7
2015
```

```output2
0
```

## 提示
Central Europe Regional Contest 2015 Problem D

