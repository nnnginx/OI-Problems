## 题目描述
A path is bad if and only if the colors of all edges in it are different, otherwise, the path is good.

A tree is bad if and only if there exists a path of length $k$ in it which is bad, otherwise, the tree is good.

Now we have a tree, we want to color its edges, the beauty of coloring of edges is the number of different colors we use, we want to make the beauty of coloring maximum possible, and we don't want our tree to become bad, what is maximum beauty we can reach?

## 输入格式
The first line of the input contains $n$ and $k$, the number of vertices of the tree, and the value $k$ which declares we shouldn't have a bad path of length $k$ in tree.

The following $n-1$ lines describe the edges of the tree. The $i$-th line contains two integers $u$ and $v$, denotes an edge between $u$ and $v$. It is guaranteed that these edges form a tree.

## 输出格式
Print one integer, the maximum number of colors we can use.

```input1
4 2
1 2
1 3
1 4
```

```output1
1
```

```input2
6 3
1 2
2 3
3 4
4 5
5 6
```

```output2
3
```

```input3
11 3
1 8
1 7
1 3
1 2
2 11
2 10
2 9
3 5
3 4
3 6
```

```output3
7
```

## 提示
### Constraints

- $1 \leq k \leq n \leq 10^5$
- $1 \leq k \leq 30$

