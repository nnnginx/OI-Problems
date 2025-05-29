## Description

For a permutation $a$ of order $n$, let $f(a)$ be a $(n+1)\times (n+1)$ square matrix, and $f(a)_{i,j}=\sum_{i'\geq i}[a_{i'}<j]$, all indices are $1$-indexed.

For two matrices $A, B$, we define the _distance product_ $A\otimes B$ be $(A\otimes B)_{i,j} = \min_k \left(A_{i,k}+B_{k,j}\right)$.

You are given two permutations $a, b$ of order $n$, it can be shown that there exists a unique permutation $c$ satisfying $f(a)\otimes f(b)=f(c)$, please compute $c$.

## Input

The first line contains one positive integer $n$. 

The rest two lines contain $n$ positive integers for each line, representing the permutations $a,b$ respectively.

## Output

Please output $n$ integers in one line, representing the permutation $c$.


```input1
3
1 3 2
2 1 3

```

```output1
2 3 1

```

## Limits And Hints

For $30\%$ of the dataset, it's guaranteed that $n\leq 100$.

For $100\%$ of the dataset, it's guaranteed that $1\leq n\leq 5\times 10^5$, and $a,b$ are permutations.

