## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the two versions of this problem is the constraint on $k$. You can make hacks only if all versions of the problem are solved.</span></p><p>You are given an undirected tree of $n$ nodes. Each node $v$ has a value $a_v$ written on it. You have to answer queries related to the tree.</p><p>You are given $q$ queries. In each query, you are given $5$ integers, $u_1, v_1, u_2, v_2, k$. Denote the count of nodes with value $c$ on path $u_1 \rightarrow v_1$ with $x_c$, and the count of nodes with value $c$ on path $u_2 \rightarrow v_2$ with $y_c$. If there are $z$ such values of $c$ such that $x_c \neq y_c$, output any $\min(z, k)$ such values in any order.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;�� the number of nodes in the tree.</p><p>The next line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;�� the value written on each node of the tree.</p><p>Then $n - 1$ lines follow. Each line contains two integers $u$ and $v$ ($1 \leq u, v \leq n, u \neq v$) denoting an edge of the tree. It is guaranteed that the given edges form a tree.</p><p>The next line contains one integer $q$ ($1 \leq q \leq 10^5$)&nbsp;�� the number of queries.</p><p>Then $q$ lines follow. Each line contains five integers $u_1, v_1, u_2, v_2, k$ ($1 \leq u_1, v_1, u_2, v_2 \leq n$, $k = 1$).</p></div><div class="output-specification"><p>For each query, output on a separate line. For a query, first output $\min(z, k)$ and then on the same line, output any $\min(z, k)$ values in any order which occur a different number of times in each path.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;�� the number of nodes in the tree.</p><p>The next line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;�� the value written on each node of the tree.</p><p>Then $n - 1$ lines follow. Each line contains two integers $u$ and $v$ ($1 \leq u, v \leq n, u \neq v$) denoting an edge of the tree. It is guaranteed that the given edges form a tree.</p><p>The next line contains one integer $q$ ($1 \leq q \leq 10^5$)&nbsp;�� the number of queries.</p><p>Then $q$ lines follow. Each line contains five integers $u_1, v_1, u_2, v_2, k$ ($1 \leq u_1, v_1, u_2, v_2 \leq n$, $k = 1$).</p>

## Output

<p>For each query, output on a separate line. For a query, first output $\min(z, k)$ and then on the same line, output any $\min(z, k)$ values in any order which occur a different number of times in each path.</p>





```input1
5
5 2 3 4 3
1 2
1 3
2 4
2 5
3
1 4 4 5 1
2 3 2 3 1
5 5 4 3 1
```




```output1
1 5
0
1 2
```



## Note

<p>For query $1$, the first path is $1 \rightarrow 2 \rightarrow 4$, coming across the multiset of values $\{5, 2, 4\}$. On the second path $4 \rightarrow 2 \rightarrow 5$, we have the multiset $\{4, 2, 3\}$. Two numbers&nbsp;�� $3$ and $5$ occur a different number of times, hence we print one of them.</p><p>In query $2$, there is no difference between the paths, hence we output $0$.</p><p>In query $3$, the first path is just the node $5$, resulting in the multiset $\{3\}$, and the second path $4 \rightarrow 2 \rightarrow 1 \rightarrow 3$ gives $\{4, 2, 5, 3\}$. The numbers $5$, $2$ and $4$ occur a different number of times.</p>
