## 题目描述
Farmer John has $N$ cows ($2 \le N \le 5 \cdot 10^6$) and is attempting to get them to sort a non-negative integer array $A$ of length $N$ by relying on their laziness. He has a lot of heavy boxes so he lines the cows up one behind another, where cow $i+1$ is behind cow $i$, and gives $a_i$ boxes to cow $i$ ($0 \le a_i$).

Cows are inherently lazy so they always look to pass their work off to someone else. From cow 1 to $N-1$ in order, each cow looks to the cow behind them. If cow $i$ has strictly more boxes than cow $i+1$, cow $i$ thinks this is "unfair" and gives one of its boxes to cow $i+1$. This process repeats until every cow is satisfied.

Farmer John will then note the number of boxes $b_i$ that each cow $i$ is holding and create an array $B$ out of these values. If $B = \text{sorted}(A)$, then Farmer John will be happy. Unfortunately, Farmer John forgot all but $Q$ values ($2 \le Q \le \min(N, 100)$) in $A$. Luckily, those values include the number of boxes he was going to give to the first and last cow. Each value that FJ remembers is given in the form $c_i\; v_i$ representing that $a_{c_i} = v_i$ ($1 \le c_i \le N$, $1 \le v_i \le 10^9$). Determine the number of different ways the missing values can be filled in so that he will be happy mod $10^9 + 7$.

## 输入格式
The first line contains two space-separated integers $N$ and $Q$ representing the number of cows and queries respectively.

The next $Q$ lines contain two space separated integers $c_i\; v_i$ representing that cow $c_i$ initially holds $v_i$ boxes. It is guaranteed that $c_1 = 1$, $c_Q = N$, and $c_i < c_{i+1}$ (the order of the cows is strictly increasing).

## 输出格式
Print the number of different ways modulo $10^9 + 7$ that values $a_i$ can be assigned such that Farmer John will be happy after the cows perform the lazy sort. It is guaranteed that there will be at least one valid assignment.

```input1
3 2
1 3
3 2
```

```output1
2
```

```input2
6 3
1 1
3 3
6 5
```

```output2
89
```

## 提示
### Sample 1 Explanation

In this example, FJ remembers the values at the ends of the array. The arrays $[3, 2, 2]$ and $[3, 3, 2]$ are the valid arrays that will make FJ happy at the end of the lazy sorting.

### SCORING:
- Inputs 3-4: $N,v_i\leq 100$
- Inputs 5-6: $N\leq 100$ and $v_i\leq 10^6$
- Inputs 7-9: $N\leq 2\times 10^5$ and $v_i\leq 10^6$
- Inputs 10-12: $N\leq 2\times 10^5$
- Inputs 13-15: No additional constraints.

