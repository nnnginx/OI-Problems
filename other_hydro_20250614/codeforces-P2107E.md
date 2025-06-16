## Description

<div><p><span class="tex-font-style-it">If I was also hit by an apple falling from an apple tree, could I become as good at physics as Newton?</span></p><p>To be better at physics, Ain wants to build an apple tree so that she can get hit by apples on it. Her apple tree has $n$ nodes and is rooted at $1$. She defines the <span class="tex-font-style-it">weight</span> of an apple tree as $\sum \limits_{i=1}^n \sum \limits_{j=i+1}^n \text{dep}(\operatorname{lca}(i,j))$. </p><p>Here, $\text{dep}(x)$ is defined as the number of edges on the unique shortest path from node $1$ to node $x$. $\operatorname{lca}(i, j)$ is defined as the unique node $x$ with the largest value of $\text{dep}(x)$ and which is present on both the paths $(1, i)$ and $(1, j)$.</p><p>From some old books Ain reads, she knows that Newton's apple tree's weight is around $k$, but the exact value of it is lost.</p><p>As Ain's friend, you want to build an apple tree with $n$ nodes for her, and the absolute difference between your tree's weight and $k$ should be <span class="tex-font-style-bf">at most $1$</span>, i.e. $|\text{weight} - k| \le 1$. Unfortunately, this is not always possible, in this case please report it.</p><p> </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two numbers $n,k$ ($2 \le n \le 10^5,0 \le k \le 10^{15}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>If there's at least one solution, print $n-1$ lines and each line contains two numbers $u,v$ $(1 \le u,v \le n)$ represents the apple tree.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two numbers $n,k$ ($2 \le n \le 10^5,0 \le k \le 10^{15}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>If there's at least one solution, print $n-1$ lines and each line contains two numbers $u,v$ $(1 \le u,v \le n)$ represents the apple tree.</p>





```input1|2,4,6
5
2 1
2 2
4 0
5 7
5 5
```




```output1
Yes
1 2
No
Yes
1 2
1 3
1 4
Yes
1 3
3 5
4 5
3 2
Yes
1 2
2 3
2 4
2 5
```



## Note

<p>In the first test case, we can check that the weight is $0$. This satisfies the condition because $k = 1$ and so the absolute difference is only $1$.</p><p>In the second test case, there exists no solution because there are no trees of $2$ nodes with weights of either $1, 2$ or $3$.</p>
