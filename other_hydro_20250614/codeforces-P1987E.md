## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">God's Blessing on This ArrayForces!</span></div><div class="epigraph-source">A Random Pebble</div></div><p>You are given a tree with $n$ vertices, rooted at vertex $1$. The $i$-th vertex has an integer $a_i$ written on it.</p><p>Let $L$ be the set of all direct children$^{\text{∗}}$ of $v$. A tree is called <span class="tex-font-style-it">wonderful</span>, if for all vertices $v$ where $L$ is not empty, $$a_v \le \sum_{u \in L}{a_u}.$$ In one operation, you choose any vertex $v$ and increase $a_v$ by $1$.</p><p>Find the minimum number of operations needed to make the given tree <span class="tex-font-style-it">wonderful</span>!</p><div><p>$^{\text{∗}}$ Vertex $u$ is called a direct child of vertex $v$ if: </p><ul> <li> $u$ and $v$ are connected by an edge, and </li><li> $v$ is on the (unique) path from $u$ to the root of the tree. </li></ul></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5000$)&nbsp;— the number of vertices in the tree.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the values initially written on the vertices.</p><p>The third line of each test case contains $n - 1$ integers $p_2, p_3 , \ldots, p_n$ ($1 \le p_i &lt; i$), indicating that there is an edge from vertex $p_i$ to vertex $i$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum number of operations needed to make the tree <span class="tex-font-style-it">wonderful</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5000$)&nbsp;— the number of vertices in the tree.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the values initially written on the vertices.</p><p>The third line of each test case contains $n - 1$ integers $p_2, p_3 , \ldots, p_n$ ($1 \le p_i &lt; i$), indicating that there is an edge from vertex $p_i$ to vertex $i$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum number of operations needed to make the tree <span class="tex-font-style-it">wonderful</span>.</p>





```input1|2,3,4,8,9,10
4
5
9 3 4 1 2
1 1 3 3
2
5 3
1
2
36 54
1
3
0 0 0
1 2
```




```output1
3
2
0
0
```



## Note

<p>The tree in the first test case: </p><center> <img class="tex-graphics" src="./34764/file/ue7fmFTm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You can apply the operation once on vertex $5$ and twice on vertex $2$ to get a <span class="tex-font-style-it">wonderful</span> tree.</p><p>In the second test case, you can apply the operation twice on vertex $2$ to get a <span class="tex-font-style-it">wonderful</span> tree.</p><p>In the third and fourth test cases, the tree is already <span class="tex-font-style-it">wonderful</span>, so you don't need to apply any operations.</p>
