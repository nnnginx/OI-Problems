## 题目描述
Mikaeel has got $n$ strings named $s_{1}, \ldots, s_{n}$ each consists of lower-case English letters. He wants to pick a non-empty substring of each one and concatenate them together to make a final string of size $k$. Help Mikaeel create the smallest lexicographical string possible.

## 输入格式
In the first line, you are given two integers $n$ and $k$, the number of strings and the size of the final string, respectively.

The $n$ following lines contain the sequence $s_{1}, \ldots, s_{n}$, the strings of Mikaeel.

## 输出格式
In a single line, print the smallest lexicographical string achievable.


```input1
3 5
abc
xxx
aaa
```

```output1
abcxa
```

```input2
5 6
ab
bz
zb
aa
cb
```

```output2
abbaab
```

## 提示
### Constraints

- $n, \sum_{i=1}^{n}\left|s_{i}\right| \leq 4000$
- $n \leq k \leq \sum_{i=1}^{n}\left|s_{i}\right|$

### Subtasks

| subtask | score | limits |
| :---: | :---: | :---: |
| 1 | 23 | $\forall_{1 \leq i \leq n},  \vert s_{i}\vert = \vert s_{1}\vert  \leq 10$，$1 \leq n \leq 50$ |
| 2 | 19 | $\forall_{1 \leq i \leq n}, \vert s_{i}\vert = \vert s_{1} \vert \leq 20$, $1 \leq n \leq 200$ |
| 3 | 58 | No extra limits |

