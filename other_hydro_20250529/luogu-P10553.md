## 题目描述
There is a full binary tree with $n$ levels(so it has exactly $2^n-1$ nodes). Each node has an integer ID from $1$ to $2^n-1$, and the $2^n-1$ IDs form an arrangement from $1$ to $2^n-1$, but you don't know.

You need to find the IDs of the $2^n-1$ nodes using at most $4800$ queries.

## 输入格式
The first line contains one integer $n(1\leq n\leq 10)$, the levels of the full binary tree.

To ask a query, you need to pick two nodes with IDs $u,v(1\leq u,v\leq 2^n-1)$, and print the line of the following form:

> "? u v"

After that, you will receive:

> "t"

The lowest common ancestor's ID of $u$ and $v$.

You can ask at most $4800$ queries.

If you have found the structure of the tree, print a line of the following form:

"! $f_1\ f_2\ f_3\ f_4$ ... $f_{2^n-1}$"

$f_i$ means the i-th node's father's ID. If it has no father, then $f_i=-1$.

After printing a query or the answer for a test case, do not forget to output the end of line and flush the output. Otherwise, you will get the verdict 'Idleness Limit Exceeded'. To do this, use:

`fflush(stdout)` or `cout.flush()` in C++;

`System.out.flush()` in Java;

`stdout.flush()` in Python.

The interactor in this task is not adaptive.

```input1
2

3

3

3
```

```output1

? 1 2

? 2 3

? 1 3

! 3 3 -1
```

## 提示
In this case, the tree's root is $3$, it's two sons are $1$ and $2$.

For any query "? a b",if $a\neq b$, the jury will return answer $3$.

So we found the tree's root is $3$ .

