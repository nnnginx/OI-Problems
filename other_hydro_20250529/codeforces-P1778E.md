## Description

<div><p>Recently, a tree has fallen on Bob's head from the sky. The tree has $n$ nodes. Each node $u$ of the tree has an integer number $a_u$ written on it. But the tree has no fixed root, as it has fallen from the sky.</p><p>Bob is currently studying the tree. To add some twist, Alice proposes a game. First, Bob chooses some node $r$ to be the root of the tree. After that, Alice chooses a node $v$ and tells him. Bob then can pick one or more nodes from the subtree of $v$. His score will be the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all the values written on the nodes picked by him. Bob has to find the maximum score he can achieve for the given $r$ and $v$.</p><p>As Bob is not a good problem-solver, he asks you to help him find the answer. Can you help him? You need to find the answers for several combinations of $r$ and $v$ for the same tree.</p><p>Recall that a tree is a connected undirected graph without cycles. The subtree of a node $u$ is the set of all nodes $y$ such that the simple path from $y$ to the root passes through $u$. Note that $u$ is in the subtree of $u$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line contains an integer $n$ ($2\leq n\leq 2 \cdot 10^5$)&nbsp;！ the number of nodes of the tree. </p><p>The next line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1\leq a_i\leq 10^9$)&nbsp;！ the values written on the nodes. </p><p>Each of the next $n-1$ lines contain two integers $u$ and $v$ ($1\leq u, v\leq n$; $u\neq v$), denoting there is an undirected edge between node $u$ and node $v$. It is guaranteed that the given edges form a tree.</p><p>The next line contains an integer $q$ ($1\leq q\leq 2 \cdot 10^5$)&nbsp;！ the number of queries. </p><p>Each of the next $q$ lines contains two integers $r$ and $v$ ($1\leq r, v\leq n$)&nbsp;！ the root node Bob defines, and the node Alice chooses.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases don't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, in each query, print a line containing an integer denoting the maximum score Bob can achieve.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line contains an integer $n$ ($2\leq n\leq 2 \cdot 10^5$)&nbsp;！ the number of nodes of the tree. </p><p>The next line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1\leq a_i\leq 10^9$)&nbsp;！ the values written on the nodes. </p><p>Each of the next $n-1$ lines contain two integers $u$ and $v$ ($1\leq u, v\leq n$; $u\neq v$), denoting there is an undirected edge between node $u$ and node $v$. It is guaranteed that the given edges form a tree.</p><p>The next line contains an integer $q$ ($1\leq q\leq 2 \cdot 10^5$)&nbsp;！ the number of queries. </p><p>Each of the next $q$ lines contains two integers $r$ and $v$ ($1\leq r, v\leq n$)&nbsp;！ the root node Bob defines, and the node Alice chooses.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases don't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, in each query, print a line containing an integer denoting the maximum score Bob can achieve.</p>





```input1|2,3,4,5,6,7,8,9,10,11,12,21,22,23,24,25,26,27
3
6
12 12 8 25 6 1
1 5
1 2
2 6
2 3
2 4
3
4 2
3 5
1 2
2
3 8
1 2
4
2 2
2 1
1 2
1 1
3
3 8 7
1 2
2 3
2
2 2
2 1
```




```output1
15
6
29
11
3
8
11
15
3
```



## Note

<p>In each of the below figures, the green-colored node is the node picked by Bob, and the red-colored node is the node picked by Alice. The values of the nodes are placed in the blue boxes beside the nodes.</p><p>Consider the first example. In the first query, if we put the root node $4$ at the top of the tree, the tree looks like the below figure: </p><center> <img class="tex-graphics" src="./33520/file/KCIS4iKE.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Tree with root node $4$ in the first query.</span> </center> The nodes in the subtree of the node $2$ are $[2,1,5,6,3]$. Among them, Bob can pick node $3$, node $5$, and node $6$. His score will be $a_3 \oplus a_5 \oplus a_6 = 8 \oplus 6 \oplus 1 = 15$. He can't achieve any score more than this.<p>In the second query, if the root node $3$ is placed at the top of the tree, the tree looks like the below figure: </p><center> <img class="tex-graphics" src="./33520/file/Wf6yXALE.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Tree with root node $3$ in the second query.</span> </center> The only node in the subtree of the node $5$ is $5$. Bob can only pick the node $5$. His score will be $a_5 = 6$.<p>In the third query, if the root node $1$ is placed at the top of the tree, the tree looks like this: </p><center> <img class="tex-graphics" src="./33520/file/gba7UuA2.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Tree with root node $1$ in the third query.</span> </center> The nodes in the subtree of the node $2$ are $[2,3,6,4]$. Among them, Bob can pick node $2$, node $3$, and node $4$. His score will be $a_2 \oplus a_3 \oplus a_4 = 12 \oplus 8 \oplus 25 = 29$. He is not able to score higher than that.
