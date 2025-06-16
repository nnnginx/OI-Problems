## 题目描述

Given an $m \times n$ grid, you're required to fill it with the numbers from $1$ to $m \times n$ but the following rules should be satisfied:  
1. each number in grid is larger than its above;  
2. each number in grid is larger than its left.  

Now, I wonder how many distinct solutions I could make on a grid.    
For example. Consider such a $2 \times 3$ grid, we have the following solutions:  
123  124  134  135  125  
456  356  256  246  346  
Thus, the sum is $5$. 

## 输入格式

Two positive integer $m, n (0 < m, n < 10)$ per line. Two zeros indicate the end of input.

## 输出格式

A single integer per line for each case -- the number of distinct solutions.


```input1
2 3
0 0
```
```output1
5
```

## 提示

本题为多组数据，请做到 `0 0` 结束。

## 题目来源

没有写明来源。