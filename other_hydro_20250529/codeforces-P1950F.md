## Description

<div><p>Find the minimum height of a rooted tree$^{\dagger}$ with $a+b+c$ vertices that satisfies the following conditions: </p><ul> <li> $a$ vertices have exactly $2$ children, </li><li> $b$ vertices have exactly $1$ child, and </li><li> $c$ vertices have exactly $0$ children. </li></ul> If no such tree exists, you should report it.<center> <img class="tex-graphics" src="./34542/file/8QsVO5P7.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">The tree above is rooted at the top vertex, and each vertex is labeled with the number of children it has. Here $a=2$, $b=1$, $c=3$, and the height is $2$.</span> </p></center><p>$^{\dagger}$ A <span class="tex-font-style-it">rooted tree</span> is a connected graph without cycles, with a special vertex called the <span class="tex-font-style-it">root</span>. In a rooted tree, among any two vertices connected by an edge, one vertex is a parent (the one closer to the root), and the other one is a child. </p><p>The <span class="tex-font-style-it">distance</span> between two vertices in a tree is the number of edges in the shortest path between them. The <span class="tex-font-style-it">height</span> of a rooted tree is the maximum distance from a vertex to the root.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains three integers $a$, $b$, and $c$ ($0 \leq a, b, c \leq 10^5$; $1 \leq a + b + c$).</p><p>The sum of $a + b + c$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if no such tree exists, output $-1$. Otherwise, output one integer&nbsp;！ the minimum height of a tree satisfying the conditions in the statement.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains three integers $a$, $b$, and $c$ ($0 \leq a, b, c \leq 10^5$; $1 \leq a + b + c$).</p><p>The sum of $a + b + c$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, if no such tree exists, output $-1$. Otherwise, output one integer&nbsp;！ the minimum height of a tree satisfying the conditions in the statement.</p>





```input1|2,4,6,8,10
10
2 1 3
0 0 1
0 1 1
1 0 2
1 1 3
3 1 4
8 17 9
24 36 48
1 0 0
0 3 1
```




```output1
2
0
1
1
-1
3
6
-1
-1
3
```



## Note

<p>The first test case is pictured in the statement. It can be proven that you can't get a height smaller than $2$.</p><p>In the second test case, you can form a tree with a single vertex and no edges. It has height $0$, which is clearly optimal.</p><p>In the third test case, you can form a tree with two vertices joined by a single edge. It has height $1$, which is clearly optimal.</p>
