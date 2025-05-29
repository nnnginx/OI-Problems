## 题目描述
You are a tourist who wishes to explore some cities. There are $n + 1$ cities, numbered from $1$ to $n + 1$ in sequence. There are some buses and trains running between these cities.

To travel between cities $i$ and $i + 1$, you have two transportation options:

- Take a train, which takes $a[i]$ units of time.
- Take a bus, which takes $b[i]$ units of time.

Determine the minimum total time required to travel from city $1$ to city $n + 1$.

## 输入格式
Your program must read from standard input.

The first line of input contains one integer $n$.

The following $n$ lines of input each contain one integer. The $i$-th of these lines contains $a[i]$.

The following $n$ lines of input each contain one integer. The $i$-th of these lines contains $b[i]$.


## 输出格式
Your program must print to standard output.

Output a single integer, the shortest time taken to travel from city $1$ to city $n + 1$.

The output should contain only a single integer. Do not print any additional text such as `Enter a number` or `The answer is`.


```input1
3
7
7
5
9
8
1
```

```output1
15
```

## 提示
## Subtasks

For all testcases, the input will satisfy the following bounds:

- $1 \leq n \leq 10$
- $1 \leq a[i] \leq 10$ for all $1 \leq i \leq n$
- $1 \leq b[i] \leq 10$ for all $1 \leq i \leq n$

Your program will be tested on input instances that satisfy the following restrictions:

| Subtask | Marks | Additional Constraints |
| :-: | :-: | :-: |
| $0$ | $0$ | Sample test cases |
| $1$ | $100$ | No additional constraints |

## Sample Test Case 1 Explanation

You start at city $1$. You then:

- Take the train from city $1$ to city $2$ ($7$ units of time taken).
- Take the train from city $2$ to city $3$ ($7$ units of time taken).
- Take the bus from city $3$ to city $4$ ($1$ unit of time taken).

The total time taken is $15$.


