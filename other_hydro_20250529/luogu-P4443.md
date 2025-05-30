## 题目背景
原题每个点4s，但我改不了= =，不过标程1s不到就过了。

## 题目描述
The biggest event of the year ended tragically for Croatian teams. The most influential theoretician of CERC of all time, the founder of the popular page CERC Tips, and in his free time an outstanding bass player, in his most recent performance failed to get his team to the finals.

In order to get over his existential troubles, our subject is spending time playing games of chance. He is especially interested in the following game:

You are given a positive integer M. Our protagonist sees in front of him a **permutation** of an array of numbers 0, 1, 2, ..., $2^M$- 1.

The computer chooses a **nonempty contiguous subsequence** of the given permutation, which it then lights up over a capital city of one of the countries in Southeastern Europe.

Our confidant, after fighting off tears caused by memories of old times, **must** choose two distinct elements of the permutation and **swap their places**​. Our man of the hour wins if and only if the **bitwise XOR** of the numbers in the lit up subsequence after the substitution is **precisely**​ $2^M$- 1.

Our hero wants to know **the number of contiguous subsequences** ​the computer can light up so that he can win.

Help our hero overcome his (id)entity crisis so our favourite page can be fully active again.


## 输入格式
The first line of input contains the integer M (1 ≤ M ≤ 20),

The following line contains $2^M$ space-separated numbers that make up a permutation of the array 0, 1, 2, ..., $2^M$- 1.


## 输出格式
You must output the total number of contiguous subsequences that a computer can light up so our hero can win.


## 题目大意
给出一个长度为2^M的排列，元素分别是0， 1， 2， ... , 2^M -1。
选择其中某个非空连续子序列，然后允许交换这个排列中某两个不同的数，然后使得这个连续子序列的所有数的按位异或(bitwise XOR)的结果恰好等于2^M-1
求：有多少个连续子序列满足上述条件。




```input1
2
0 1 2 3

```

```output1
9
```

```input2
3
3 7 0 4 6 1 5 2

```

```output2
33
```

```input3
4
13 0 15 12 4 8 7 3
11 14 6 10 1 5 9 2

```

```output3
133
```

## 提示
In test cases worth 50% of total points, it will hold 1 ≤ M ≤ 14.

**Clarification​ ​of​ ​the​ ​test​ ​cases:**

In the first test case, if the computer chooses the subsequence [1 2 3], our hero can replace the numbers 0 and 3. In this case, he can actually win for every chosen contiguous subsequence, except the entire array.

In the second test case, if the computer chooses the entire array [3 7 0 4 6 1 5 2] as the lit up subsequence, our hero can’t change the XOR of the subsequence (which is 0), no matter which two elements are swapped.

