## Description

<div><p><span class="tex-font-style-bf">Easy and hard versions are actually different problems, so we advise you to read both statements carefully</span>.</p><p>You are given a weighted rooted tree, vertex $1$ is the root of this tree.</p><p>A tree is a connected graph without cycles. A rooted tree has a special vertex called the root. A parent of a vertex $v$ is the last different from $v$ vertex on the path from the root to the vertex $v$. Children of vertex $v$ are all vertices for which $v$ is the parent. A vertex is a leaf if it has no children. The weighted tree is such a tree that each edge of this tree has some weight.</p><p>The weight of the path is the sum of edges weights on this path. The weight of the path from the vertex to itself is $0$.</p><p>You can make a sequence of zero or more moves. On each move, you select an edge and divide its weight by $2$ rounding down. More formally, during one move, you choose some edge $i$ and divide its weight by $2$ rounding down ($w_i := \left\lfloor\frac{w_i}{2}\right\rfloor$).</p><p>Your task is to find the minimum number of <span class="tex-font-style-bf">moves</span> required to make the <span class="tex-font-style-bf">sum of weights of paths</span> from the root to each leaf at most $S$. In other words, if $w(i, j)$ is the weight of the path from the vertex $i$ to the vertex $j$, then you have to make $\sum\limits_{v \in leaves} w(root, v) \le S$, where $leaves$ is the list of all leaves.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $S$ ($2 \le n \le 10^5; 1 \le S \le 10^{16}$) �� the number of vertices in the tree and the maximum possible sum of weights you have to obtain. The next $n-1$ lines describe edges of the tree. The edge $i$ is described as three integers $v_i$, $u_i$ and $w_i$ ($1 \le v_i, u_i \le n; 1 \le w_i \le 10^6$), where $v_i$ and $u_i$ are vertices the edge $i$ connects and $w_i$ is the weight of this edge.</p><p>It is guaranteed that the sum of $n$ does not exceed $10^5$ ($\sum n \le 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer: the minimum number of <span class="tex-font-style-bf">moves</span> required to make the sum of weights of paths from the root to each leaf at most $S$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $S$ ($2 \le n \le 10^5; 1 \le S \le 10^{16}$) �� the number of vertices in the tree and the maximum possible sum of weights you have to obtain. The next $n-1$ lines describe edges of the tree. The edge $i$ is described as three integers $v_i$, $u_i$ and $w_i$ ($1 \le v_i, u_i \le n; 1 \le w_i \le 10^6$), where $v_i$ and $u_i$ are vertices the edge $i$ connects and $w_i$ is the weight of this edge.</p><p>It is guaranteed that the sum of $n$ does not exceed $10^5$ ($\sum n \le 10^5$).</p>

## Output

<p>For each test case, print the answer: the minimum number of <span class="tex-font-style-bf">moves</span> required to make the sum of weights of paths from the root to each leaf at most $S$.</p>

## Samples

```input1
3
3 20
2 1 8
3 1 7
5 50
1 3 100
1 5 10
2 3 123
5 4 55
2 100
1 2 409
```

```output1
0
8
3
```



