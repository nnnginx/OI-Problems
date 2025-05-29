## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. In this version, the given tree is a perfect binary tree and the constraints on $n$ and $q$ are lower. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given a perfect binary tree$^\dagger$ consisting of $n$ vertices. The vertices are numbered from $1$ to $n$, and the root is the vertex $1$. You are also given a permutation $p_1, p_2, \ldots, p_n$ of $[1,2,\ldots,n]$.</p><p>You need to answer $q$ queries. For each query, you are given two integers $x$, $y$; you need to swap $p_x$ and $p_y$ and determine if $p_1, p_2, \ldots, p_n$ is a valid DFS order$^\ddagger$ of the given tree.</p><p>Please note that the swaps are <span class="tex-font-style-bf">persistent</span> through queries.</p><p>$^\dagger$ A perfect binary tree is a tree with vertex $1$ as its root, with size $n=2^k-1$ for a positive integer $k$, and where the parent of each vertex $i$ ($1&lt;i\le n$) is $\left\lfloor\frac{i}{2}\right\rfloor$. Thus, all leaves of this tree are at a distance $k - 1$ from the root.</p><p>$^\ddagger$ A DFS order is found by calling the following $\texttt{dfs}$ function on the given tree.</p><pre class="lstlisting"><code class="prettyprint">dfs_order = []<br><br>function dfs(v):<br>    append v to the back of dfs_order<br>    pick an arbitrary permutation s of children of v<br>    for child in s:<br>        dfs(child)<br>dfs(1)<br></code></pre><p>Note that the DFS order is not unique.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $q$ ($3\le n\le 65\,535$, $2\le q\le 5 \cdot 10^4$)&nbsp;！ the number of vertices in the tree and the number of queries. It is guaranteed that $n=2^k-1$ for a positive integer $k$.</p><p>The next line contains $n-1$ integers $a_2,a_3,\ldots,a_n$ ($1\le a_i&lt;i$)&nbsp;！ the parent of each vertex in the given tree. It is guaranteed that $a_i=\left\lfloor\frac{i}{2}\right\rfloor$.</p><p>The next line contains $n$ integers $p_1,p_2,\ldots,p_n$ ($1\le p_i\le n$, all $p_i$ are distinct)&nbsp;！ the initial permutation $p$.</p><p>The next $q$ lines each contain two integers $x$, $y$ ($1\le x,y\le n,x\neq y$)&nbsp;！ the positions of the elements to swap in the permutation.</p><p>It is guaranteed that the sum of all $n$ does not exceed $65\,535$, and the sum of all $q$ does not exceed $5 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, print $q$ lines corresponding to the $q$ queries. For each query, output $\texttt{YES}$ if there is a DFS order that exactly equals the current permutation, and output $\texttt{NO}$ otherwise.</p><p>You can output $\texttt{Yes}$ and $\texttt{No}$ in any case (for example, strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$ and $\texttt{YES}$ will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $q$ ($3\le n\le 65\,535$, $2\le q\le 5 \cdot 10^4$)&nbsp;！ the number of vertices in the tree and the number of queries. It is guaranteed that $n=2^k-1$ for a positive integer $k$.</p><p>The next line contains $n-1$ integers $a_2,a_3,\ldots,a_n$ ($1\le a_i&lt;i$)&nbsp;！ the parent of each vertex in the given tree. It is guaranteed that $a_i=\left\lfloor\frac{i}{2}\right\rfloor$.</p><p>The next line contains $n$ integers $p_1,p_2,\ldots,p_n$ ($1\le p_i\le n$, all $p_i$ are distinct)&nbsp;！ the initial permutation $p$.</p><p>The next $q$ lines each contain two integers $x$, $y$ ($1\le x,y\le n,x\neq y$)&nbsp;！ the positions of the elements to swap in the permutation.</p><p>It is guaranteed that the sum of all $n$ does not exceed $65\,535$, and the sum of all $q$ does not exceed $5 \cdot 10^4$.</p>

## Output

<p>For each test case, print $q$ lines corresponding to the $q$ queries. For each query, output $\texttt{YES}$ if there is a DFS order that exactly equals the current permutation, and output $\texttt{NO}$ otherwise.</p><p>You can output $\texttt{Yes}$ and $\texttt{No}$ in any case (for example, strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$ and $\texttt{YES}$ will be recognized as a positive response).</p>





```input1|2,3,4,5,6,7
2
3 3
1 1
1 2 3
2 3
3 2
1 3
7 4
1 1 2 2 3 3
1 2 3 4 5 6 7
3 5
2 5
3 7
4 6
```




```output1
YES
YES
NO
YES
NO
NO
YES
```



## Note

<p>In the first test case, the permutation $p_1, p_2, \ldots, p_n$ after each modification is $[1,3,2],[1,2,3],[3,2,1]$, respectively. The first two permutations are valid DFS orders; the third is not a DFS order.</p><p>In the second test case, the permutation $p_1, p_2, \ldots, p_n$ after each modification is $[1,2,5,4,3,6,7],[1,3,5,4,2,6,7],[1,3,7,4,2,6,5],[1,3,7,6,2,4,5]$, respectively.</p>
