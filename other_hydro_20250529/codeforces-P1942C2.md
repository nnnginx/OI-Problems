## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/alice-law-314125270/manbo-p-proof-geometric-construction-can-solve-all-love-affairs">Proof Geometric Construction Can Solve All Love Affairs - manbo-p</a></span></div><div class="epigraph-source">⠀</div></div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference between the two versions is the constraint on $y$. In this version $0 \leq y \leq n - x$. You can make hacks only if both versions are solved.</span></p><p>Bessie has received a birthday cake from her best friend Elsie, and it came in the form of a regular polygon with $n$ sides. The vertices of the cake are numbered from $1$ to $n$ clockwise. You and Bessie are going to choose some of those vertices to cut <span class="tex-font-style-bf">non-intersecting</span> diagonals into the cake. In other words, the endpoints of the diagonals must be part of the chosen vertices.</p><p>Bessie would only like to give out pieces of cake which result in a triangle to keep consistency. The size of the pieces doesn't matter, and the whole cake does not have to be separated into all triangles (other shapes are allowed in the cake, but those will not be counted). </p><p>Bessie has already chosen $x$ of those vertices that can be used to form diagonals. She wants you to choose <span class="tex-font-style-bf">no more than</span> $y$ other vertices such that the number of triangular pieces of cake she can give out is maximized.</p><p>What is the maximum number of triangular pieces of cake Bessie can give out?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case consists of three integers, $n$, $x$, and $y$ ($4 \leq n \leq 10^9$, $2 \leq x \leq \min(n, 2 \cdot 10^5)$, $0 \leq y \leq n - x$)&nbsp;— the number of sides of the polygon, number of vertices Bessie has chosen, and the maximum number of other vertices you can choose.</p><p>The second line consists of $x$ distinct integers from $1$ to $n$, representing the vertices Bessie has chosen.</p><p>It is guaranteed the sum of $x$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer: the maximum number of non-intersecting triangular pieces of cake she can give out.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case consists of three integers, $n$, $x$, and $y$ ($4 \leq n \leq 10^9$, $2 \leq x \leq \min(n, 2 \cdot 10^5)$, $0 \leq y \leq n - x$)&nbsp;— the number of sides of the polygon, number of vertices Bessie has chosen, and the maximum number of other vertices you can choose.</p><p>The second line consists of $x$ distinct integers from $1$ to $n$, representing the vertices Bessie has chosen.</p><p>It is guaranteed the sum of $x$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output a single integer: the maximum number of non-intersecting triangular pieces of cake she can give out.</p>





```input1|2,3,6,7
3
8 4 2
1 6 2 5
7 3 1
6 4 3
4 2 2
1 3
```




```output1
6
5
2
```



## Note

<p>In test cases $1$, $2$ and $3$, you can get $6$, $5$ and $2$ non-intersecting triangular pieces of cake, respectively. A possible construction is shown in the following pictures:</p><p>The green dots represent vertices that Bessie chose, the yellow dots represent vertices that you chose, the blue lines represent diagonals that are drawn, and the red numbers represent triangles that are counted.</p><center> <img class="tex-graphics" src="./34489/file/1su6W33h.png" style="max-width: 100.0%;max-height: 100.0%;">   </center>
