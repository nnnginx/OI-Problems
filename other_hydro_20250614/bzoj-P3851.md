## 题目描述

Teacher Mai is addicted to game 2048. But finally he finds it's too hard to get 2048. So he wants to change the rule:
You are given some numbers. Every time you can choose two numbers of the same value from them and merge these two numbers into their sum. And these two numbers disappear meanwhile.

If we can get 2048 from a set of numbers with this operation, Teacher Mai think this multiset is good.
You have $n$ numbers, $A_1,...,A_n$. Teacher Mai ask you how many subsequences of $A$ are good.
The number can be very large, just output the number $\bmod$ $998244353$.

## 输入格式

There are multiple test cases, terminated by a line "0".
For each test case, the first line contains an integer $n$ $(1 \le n \le 10^5)$, the next line contains $n$ integers $a_i$ $(0 \le ai \le 2048)$.

## 输出格式

For each test case, output one line "Case #k: ans", where $k$ is the case number counting from $1$ , ans is the number $\bmod$ $998244353$.

```input14
1024 512 256 256
4
1024 1024 1024 1024
5
1024 512 512 512 1
0
```

```output1Case #1: 1
Case #2: 11
Case #3: 8
```

## 提示

In the first case, we should choose all the numbers.
In the second case, all the subsequences which contain more than one number are good.


