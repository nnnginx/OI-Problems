## 题目描述
Someday Shayan had a graph with $n$ vertices, vertices were labeled by numbers 1 to $n$, but it has got stolen from him.

Thieves have sent him $n$ pictures of the graph, in each picture exactly one of the vertices is removed, and labels of other vertices are re-indexed from 1 to $n-1$ (each vertex will being removed in exactly one of the graphs).

The thieves have told him if he can tell the size of connected components of the graph, They will give the graph back to him, but sadly Shayan does not remember the answer to this question, so he asked you to help him find the answer.

## 输入格式
First line contains the number $n$, number of vertices of the graph.

The following lines are the descriptions of the $n$ pictures. The $i$-th graph starts with number $m_i$, the number of edges in the graph without a specific vertex. The vertices are randomly shuffled and are indexed between 1 to $n-1$. The next $m_i$ lines contain the description of the edges.

It is guaranteed that the input is not self contradictory.

## 输出格式
In the first line of output print the number of connected components of the graph. In the next line, print the sizes of the components in the non-decreasing order.

```input1
3
1
1 2
1
1 2
1
1 2
```

```output1
1
3
```

```input2
5
2
1 2
3 1
1
1 2
2
2 3
1 4
2
2 4
3 4
2
1 2
3 4
```

```output2
2
2 3
```

## 提示
### Constraints

- $1 \leq n \leq 300$
- $0 \leq m_i \leq \binom{n-1}{2}$
- $1 \leq v_i, u_i \leq n - 1$

### Subtasks

| subtask | score | limits |
|:---------:|:-------:|:--------:|
| 1       | 100   | No extra limits |

