## 题目描述
Penguinland is an infinite number line with n monsters. The $i$-th monster is initially at position $a[i]$ on the number line, with health $h[i]$. It is guaranteed that no two monsters share the same initial position.

Today, Brian the penguin wishes to defeat all the monsters! To defeat them, Brian has planted $k$ mines at certain positions. The $j$-th mine is located at position $x[j]$. Detonating a mine **instantly destroys all monsters** standing on that position, and each mine can be detonated any number of times. However, each detonation costs $1$ dollar. It is guaranteed that no two mines are planted at the same position.

In addition to detonating mines, Brian can also perform two types of operations:

- Move a monster left or right by $1$ unit along the number line.
- Increase or decrease a monster’s health by $1$.

Each operation costs $1$ dollar to execute.

A monster is considered defeated if its health reaches $0$ or if it is destroyed by a mine. Help Brian find the minimum cost (in dollars) needed to defeat all the monsters.


## 输入格式
Your program must read from standard input.

The first line of input contains two space-separated integers $n$ and $k$.

The following $n$ lines each contain two space-separated integers. The $i$-th of these lines contains $a[i]$ and $h[i]$.

The last line of input contains $k$ space-separated integers $x[1], x[2], \ldots, x[k]$.


## 输出格式
Your program must print to standard output.

Output a single integer, the minimum cost (in dollars) needed to defeat all the monsters.

The output should contain only a single integer. Do not print any additional text such as Enter a number or The answer is.


```input1
3 1
2 2
4 5
5 4
5
```

```output1
4
```

```input2
5 2
7 7
6 3
10 4
4 4
9 1
7 10
```

```output2
7
```

```input3
10 5
19 10
5 3
1 2
3 6
17 2
20 3
8 2
12 3
14 2
15 1
40 13 37 14 6
```

```output3
23
```

## 提示
### Subtasks

For all test cases, the input will satisfy the following bounds:

- $1 \leq n, k \leq 200\,000$
- $1 \leq a[i], h[i] \leq 10^9$ for all $1 \leq i \leq n$
- $1 \leq x[i] \leq 10^9$ for all $1 \leq i \leq k$
- $a[i] \neq a[j]$ for all $i \neq j$
- $x[i] \neq x[j]$ for all $i \neq j$

Your program will be tested on input instances that satisfy the following restrictions:

| Subtask | Marks | Additional constraints |
| :-: | :-: | :-: |
| $0$ | $0$ | Sample test cases |
| $1$ | $14$ | $k = 1$ |
| $2$ | $6$ | $k = 2$ |
| $3$ | $10$ | $n, k \leq 18$ |
| $4$ | $30$ | $n, k \leq 3000$ |
| $5$ | $29$ | $h[i] = 10^9$ |
| $6$ | $11$ | No additional constraints |

### Sample Test Case 1 Explanation

There are $n = 3$ monsters and $k = 1$ mine. Brian can:

- Decrease the health of monster $1$ to $0$, costing $2$ dollars.
- Move monster $2$ to the right by $1$ unit (changing its position from $4$ to $5$), costing $1$ dollar.
- Detonate the mine at position $5$, defeating both monsters $2$ and $3$, costing $1$ dollar.

The total cost needed is $2 + 1 + 1 = 4$ dollars.

This test case is valid for subtasks $1, 3, 4$, and $6$.

### Sample Test Case 2 Explanation

This test case is valid for subtasks $2, 3, 4$, and $6$.

There are $n = 5$ monsters and $k = 2$ mines. Brian can:

- Decrease the health of monster $5$ to $0$, costing $1$ dollar.
- Detonate mine $2$, defeating monster $3$, costing $1$ dollar.
- Move monster $2$ to the right by $1$ unit (changing its position from $6$ to $7$), costing $1$ dollar.
- Move monster $4$ to the right by $3$ units (changing its position from $4$ to $7$), costing $3$ dollars.
- Detonate mine $1$, defeating monsters $1, 2$, and $4$, costing $1$ dollar.

The total cost needed is $1 + 1 + 1 + 3 + 1 = 7$ dollars.

### Sample Test Case 3 Explanation

This test case is valid for subtasks $3, 4$, and $6$.


