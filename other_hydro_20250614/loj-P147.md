## Description

This is a templete problem.

Warning: Large IO data. Please use fast IO, and use Tarjan Algorithm or HLD to find LCA.

Given a rooted tree with $N$ vertices, numbered from $1$ to $N$. The root is at vertex $R$. Each vertex has a value, the value of vertex $i$ is $v_i$.

There are $M$ operations to the tree in 3 types:

* `1 a x`, add $x$ to the value of vertex $a$;
* `2 a x`£¬add $x$ to each value in subtree $a$;
* `3 a b`£¬output the sum of values in the simple path from vertex $a$ to vertex $b$.

## Input

The first line contains three integers $N,M$ and $R$.  
The second line contains $N$ integers $v_1,$ $v_2,$ $\ldots,$ $v_N$.  
Each of the next $N-1$ lines contains two numbers, representing an edge.  
Each of the next $M$ contains an operation.

## Output

For each `3 a b` operation, output a single integer, representing the sum of values in the simple path from vertex $a$ to vertex $b$.

```input1
10 13 5
-2 -7 0 2 -9 -2 -4 9 8 -1
9 8
9 4
9 2
4 10
10 7
10 6
2 1
8 3
7 5
3 8 6
1 7 -8
1 5 -9
1 5 -4
1 4 -2
1 2 -1
3 5 1
1 7 1
3 1 3
1 1 -3
3 10 2
1 1 -8
3 8 4
```

```output1
16
-37
7
-1
17
```

## Limits And Hints

$40\%$ of the test cases do not have any `2 a x` operation.  
All test cases satisfies $1\leqslant N, M\leqslant 10^6,$ $1\leqslant R\leqslant N,$ $-10^6\leqslant v_i, x\leqslant 10^6$.

