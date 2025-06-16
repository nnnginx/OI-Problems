## 题目描述
You have a rooted tree with $n$ vertices, each assigned a value $a_x$. The root is node $1$. 

You can perform operations where you merge two adjacent nodes $x$ and $y$ into a single node $z$, with the value of $z$ being equal to the minimum value between the two nodes. This operation changes edges connected to $x$ or $y$ to be connected to $z$. The cost of this operation is $|a_x - a_y|$. The total cost of multiple operations is the sum of individual operation costs.

For queries, you have two types:
- $1\ x\ y$: This updates the value of node $x$ to $y$.
- $2\ x$: This asks for the minimum cost of operations to reduce the subtree rooted at $x$ to just one node.

## 输入格式
The first line contains a single integer $n$ $(1 \le n \le 200\,000)$, the number of vertices.

The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^9)$, representing the assigned values of each node.

The third line contains $n-1$ integers $p_2, p_3, \dots, p_n$ ($1 \leq p_i \leq n$), representing the parent of each node.

The fourth line contains one integer $q$ $(1 \le q \le 200\,000)$, representing the total number of queries.

The following $q$ lines each contain a query:

Either $1\ x\ y$ ($1 \leq x \leq n$, $1\leq y \leq 10^9$), or $2\ x$ ($1\leq x \leq n$).

## 输出格式
On each line of the input, you need to print the result of a query of type $2$, in the same order as the order from the input.

```input1
7
4 7 9 7 4 1 2
1 1 3 2 3 2
1
2 1
```

```output1
11
```

```input2
7
6 6 5 1 6 6 4
1 1 2 3 3 3
3
2 1
1 1 1
2 1
```

```output2
7
11
```

## 提示
- ($4$ points) $n \le 1000, q=1$;
- ($13$ points) $q=1$;
- ($15$ points) the tree is a chain and there are only queries of the second type;
- ($24$ points) there are only queries of the second type;
- ($12$ points) $p_i=1$;
- ($32$ points) no additional constraints.

