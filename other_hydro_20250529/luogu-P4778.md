## 题目背景
Just like yesterday (in problem U of the practice session), Bob is busy, so Alice keeps on playing some single-player games and puzzles. In her newest puzzle she has a permutation of numbers from 1 to n. The goal of the puzzle is to sort the permutation using the smallest possible number of swaps.    

Instead of simply solving the puzzle, Alice is wondering about the probability of winning it just by playing at random. In order to answer this question, she needs to know the number of optimal solutions to her puzzle.    

## 题目描述
You are given a permutation p1, …, pn of the numbers 1 through n. In each step you can choose two numbers x < y and swap px with py.  

Let m be the minimum number of such swaps needed to sort the given permutation. Compute the number of different sequences of exactly m swaps that sort the given permutation. Since this number may be large, compute it modulo 10^9 + 9.  

## 输入格式
The first line of the input file contains an integer t specifying the number of test cases. Each test case is preceded by a blank line.  

Each test case consists of two lines. The first line contains the integer n. The second line contains the sequence p1, …, pn: a permutation of 1, …, n.  

In the easy subproblem C1, 1 ≤ n ≤ 10.  

In the hard subproblem C2, 1 ≤ n ≤ 105.  

## 输出格式
For each test case, output a single line with a single integer: x%(10^9+9), where x is the number of ways to sort the given sequence using as few swaps as possible.  

## 题目大意
给定你一个 $ 1∼n $ 的排列 $p$，可进行若干次操作，每次选择两个整数 $x,y$，交换 $px,py$。

请你告诉穰子，用最少的操作次数将给定排列变成单调上升的序列 $1,2,…,n$，有多少种方式呢？请输出方式数对 $10^9+9$ 取模的结果。

Translated by @LJC00118 

```input1
3

3
2 3 1

4
2 1 4 3

2
1 2
```

```output1
3
2
1
```

## 提示
In the first test case, we can sort the permutation in two swaps. We can make the first swap arbitrarily; for each of them, there’s exactly one optimal second swap. For example, one of the three shortest solutions is “swap p1 with p2 and then swap p1 with p3”.  

In the second test case, the optimal solution involves swapping p1 with p2 and swapping p3 with p4. We can do these two swaps in either order.  

The third sequence is already sorted. The optimal number of swaps is 0, and thus the only optimal solution is an empty sequence of swaps.  
题目来源：[IPSC2016](https://ipsc.ksp.sk/2016/real/problems/c.html)

