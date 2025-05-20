Farmer John's cows have been holding a daily online gathering on the "mooZ" video meeting platform. For fun, they have invented a simple number game to play during the meeting to keep themselves entertained.

Elsie has three positive integers $A$, $B$, and $C$ ($1\leqslant A\leqslant B\leqslant C$). These integers are supposed to be secret, so she will not directly reveal them to her sister Bessie. Instead, she tells Bessie $N$ distinct integers $x_1,x_2,\ldots,x_N$, claiming that each $x_i$ is one of $A$, $B$, $C$, $A+B$, $B+C$, $C+A$, or $A+B+C$. However, Elsie may be lying; the integers $x_i$ might not correspond to any valid triple $(A,B,C)$.

This is too hard for Bessie to wrap her head around, so it is up to you to determine the number of triples $(A,B,C)$ that are consistent with the numbers Elsie presented (possibly zero).

Each input file will contain $T$ test cases that should be solved independently.

> - $1\leqslant x_i\leqslant 10^9$
> - $4\leqslant N\leqslant 7$
> - $1\leqslant T\leqslant 100$

## Input Format

The first input line contains $T$.

Each test case starts with $N$, the number of integers Elsie gives to Bessie.

The second line of each test case contains $N$ distinct integers $x_1,x_2,\ldots,x_N$.


## Output Format

For each test case, output the number of triples $(A,B,C)$ that are consistent with the numbers Elsie presented.

```input1
10
7
1 2 3 4 5 6 7
4
4 5 7 8
4
4 5 7 9
4
4 5 7 10
4
4 5 7 11
4
4 5 7 12
4
4 5 7 13
4
4 5 7 14
4
4 5 7 15
4
4 5 7 16
```
```output1
1
3
5
1
4
3
0
0
0
1
```

> For $x=\{4,5,7,9\}$, the five possible triples are as follows:
> 
> $$(2, 2, 5), (2, 3, 4), (2, 4, 5), (3, 4, 5), (4, 5, 7).$$

## Scoring

- In test cases 1-4, all $x_i$ are at most $50$.
- Test cases 5-6 satisfy $N=7$.
- Test cases 7-15 satisfy no additional constraints.

## Problem Credits

Benjamin Qi