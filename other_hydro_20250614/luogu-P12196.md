```input1
3 10 10
2 5 9
1 3 1
4 7 10
```

```output1
6
```

```input2
10 10 50
8 8 0
3 3 0
6 6 2
7 7 9
1 1 50
5 5 21
6 6 4
10 10 4
10 10 3
10 10 3
```

```output2
9
```

```input3
4 17 0
2 4 1000000000
6 9 1000000000
8 13 1000000000
15 16 1000000000
```

```output3
4
```

## 提示
### Subtasks

For all testcases, the input will satisfy the following bounds:

- $1 \leq h, w \leq 2000$
- $0 \leq k \leq 10^9$
- $1 \leq l[i] \leq r[i] \leq w$ for all $1 \leq i \leq h$
- $0 \leq c[i] \leq 10^9$ for all $1 \leq i \leq h$

Your program will be tested on input instances that satisfy the following restrictions:

| Subtask | Marks | Additional constraints |
| :-: | :-: | :-: |
| $0$ | $0$ | Sample test cases |
| $1$ | $6$ | $k = 0, c[i] = 10^9$ |
| $2$ | $9$ | $l[i] = r[i]$ |
| $3$ | $10$ | $h, w \leq 18$ |
| $4$ | $7$ | $h, w \leq 100, k \leq 2000$ |
| $5$ | $15$ | $h, w \leq 100$ |
| $6$ | $23$ | $h, w \leq 500$ |
| $7$ | $8$ | $r[1] − l[1] = r[2] − l[2] = \ldots = r[h] − l[h]$ |
| $8$ | $22$ | No additional constraints |

### Sample Test Case 1 Explanation

This test case is valid for subtasks $3, 4, 5, 6$, and $8$.

The laser toy in the above figure corresponds to this test case. Pavement can unlock the first and second sliding walls for a total cost of $9 + 1 = 10$ dollars. He can then slide the first sliding wall such that it spans columns $4$ to $7$, and slide the second sliding wall to span columns $5$ to $7$.

![](https://cdn.luogu.com.cn/upload/image_hosting/glj93dtp.png)

This leaves $6$ lasers (in columns $1, 2, 3, 8, 9$, and $10$) unblocked, which is the maximum possible.

### Sample Test Case 2 Explanation

This test case is valid for subtasks $2$ to $8$.

### Sample Test Case 3 Explanation

This test case is valid for subtasks $1, 3, 4, 5, 6$, and $8$.

