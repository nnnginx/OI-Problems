


## 题目描述
给一列数，要求支持操作： 1.修改某个数的值 2.读入l,r,k，询问在[l,r]内选不相交的不超过k个子段，最大的和是多少。
## 输入格式
The first line contains integer n (1 ≤ n ≤ 10^{5}), showing how many numbers the sequence has. The next line contains n integers a_{1}, a_{2}, ..., a_{n} (|a_{i}| ≤ 500). 
The third line contains integer m (1 ≤ m ≤ 10^{5}) — the number of queries. The next m lines contain the queries in the format, given in the statement.
All changing queries fit into limits: 1 ≤ i ≤ n, |val| ≤ 500.
All queries to count the maximum sum of at most k non-intersecting subsegments fit into limits: 1 ≤ l ≤ r ≤ n, 1 ≤ k ≤ 20. It is guaranteed that the number of the queries to count the maximum sum of at most k non-intersecting subsegments doesn't exceed 10000.
## 输出格式
For each query to count the maximum sum of at most k non-intersecting subsegments print the reply — the maximum sum. Print the answers to the queries in the order, in which the queries follow in the input.

```input1
9
9 -8 9 -1 -1 -1 9 -8 9
3
1 1 9 1
1 1 9 2
1 4 6 3

```
```output1
17
25
0
```

## 提示
In the first query of the first example you can select a single pair (1, 9). So the described sum will be 17.
Look at the second query of the first example. How to choose two subsegments? (1, 3) and (7, 9)? Definitely not, the sum we could get from (1, 3) and (7, 9) is 20, against the optimal configuration (1, 7) and (9, 9) with 25.
The answer to the third query is 0, we prefer select nothing if all of the numbers in the given interval are negative.
## 题目来源
By xiaodao


