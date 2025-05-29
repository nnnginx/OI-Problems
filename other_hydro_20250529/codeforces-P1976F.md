## Description

<div><p>You are given a rooted tree, consisting of $n$ vertices, numbered from $1$ to $n$. Vertex $1$ is the root. Additionally, the root only has one child.</p><p>You are asked to add exactly $k$ edges to the tree (possibly, multiple edges and/or edges already existing in the tree).</p><p>Recall that a bridge is such an edge that, after you remove it, the number of connected components in the graph increases. So, initially, all edges of the tree are bridges.</p><p>After $k$ edges are added, some original edges of the tree are still bridges and some are not anymore. You want to satisfy two conditions: </p><ul> <li> for every bridge, all tree edges in the subtree of the lower vertex of that bridge should also be bridges; </li><li> the number of bridges is as small as possible. </li></ul><p>Solve the task for all values of $k$ from $1$ to $n - 1$ and output the smallest number of bridges.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;！ the number of vertices of the tree.</p><p>Each of the next $n - 1$ lines contain two integers $v$ and $u$ ($1 \le v, u \le n$)&nbsp;！ the description of the edges of the tree. It's guaranteed that the given edges form a valid tree.</p><p>Additional constraint on the input: the root (vertex $1$) has exactly one child.</p><p>The sum of $n$ over all testcases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print $n - 1$ integers. For each $k$ from $1$ to $n - 1$ print the smallest number of bridges that can be left after you add $k$ edges to the tree.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;！ the number of vertices of the tree.</p><p>Each of the next $n - 1$ lines contain two integers $v$ and $u$ ($1 \le v, u \le n$)&nbsp;！ the description of the edges of the tree. It's guaranteed that the given edges form a valid tree.</p><p>Additional constraint on the input: the root (vertex $1$) has exactly one child.</p><p>The sum of $n$ over all testcases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each testcase, print $n - 1$ integers. For each $k$ from $1$ to $n - 1$ print the smallest number of bridges that can be left after you add $k$ edges to the tree.</p>





```input1|2,3,16,17,18,19,20,21,22,23
4
2
1 2
12
4 10
5 12
12 11
3 6
9 6
1 6
12 7
11 6
2 11
10 9
10 8
8
1 2
2 3
2 4
3 5
3 6
4 7
4 8
5
1 2
2 3
3 4
4 5
```




```output1
0 
7 3 1 0 0 0 0 0 0 0 0 
4 1 0 0 0 0 0 
0 0 0 0
```


