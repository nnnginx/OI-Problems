## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Endless Repeating 7 Days</span></div><div class="epigraph-source">— r-906, <a href="https://www.youtube.com/watch?v=_-Vd0ZGB-lo"><span class="tex-font-style-it">Panopticon</span></a></div></div><p>There is a tree consisting of $n$ vertices. Let a <span class="tex-font-style-it">caterpillar</span> be denoted by an integer pair $(p, q)$ ($1 \leq p, q \leq n$, $p \neq q$): its head is at vertex $p$, its tail is at vertex $q$, and it dominates all the vertices on the simple path from $p$ to $q$ (including $p$ and $q$). The <span class="tex-font-style-it">caterpillar sequence</span> of $(p, q)$ is defined as the sequence consisting only of the vertices on the simple path, sorted in the ascending order of the distance to $p$.</p><p>Nora and Aron are taking turns moving the <span class="tex-font-style-it">caterpillar</span>, with Nora going first. Both players will be using his or her own optimal strategy:</p><ul> <li> They will play to make himself or herself <span class="tex-font-style-it">win</span>; </li><li> However, if it is impossible, they will play to prevent the other person from <span class="tex-font-style-it">winning</span> (thus, the game will end in a <span class="tex-font-style-it">tie</span>). </li></ul><p>In Nora's turn, she must choose a vertex $u$ adjacent to vertex $p$, which is not dominated by the <span class="tex-font-style-it">caterpillar</span>, and move all the vertices in it by one edge towards vertex $u$$^{\text{∗}}$. In Aron's turn, he must choose a vertex $v$ adjacent to vertex $q$, which is not dominated by the <span class="tex-font-style-it">caterpillar</span>, and move all the vertices in it by one edge towards vertex $v$. Note that the moves allowed to the two players are different.</p><p>Whenever $p$ is a leaf$^{\text{†}}$, Nora <span class="tex-font-style-it">wins</span>$^{\text{‡}}$. Whenever $q$ is a leaf, Aron <span class="tex-font-style-it">wins</span>. If either initially both $p$ and $q$ are leaves, or after $10^{100}$ turns the game has not ended, the result is a <span class="tex-font-style-it">tie</span>.</p><p>Please count the number of integer pairs $(p, q)$ with $1 \leq p, q \leq n$ and $p \neq q$ such that, if the <span class="tex-font-style-it">caterpillar</span> is initially $(p, q)$, Aron <span class="tex-font-style-it">wins</span> the game.</p><div class="statement-footnote"><p>$^{\text{∗}}$In other words: Let the current <span class="tex-font-style-it">caterpillar sequence</span> be $c_1, c_2, \ldots, c_k$, then after the move, the new <span class="tex-font-style-it">caterpillar sequence</span> becomes $d(u, c_1), d(u, c_2), \ldots, d(u, c_k)$. Here, $d(x, y)$ is the next vertex on the simple path from $y$ to $x$.</p><p>$^{\text{†}}$In a tree, a vertex is called a leaf if and only if its degree is $1$.</p><p>$^{\text{‡}}$Therefore, Nora never fails to choose a vertex $u$ when the game has not ended. The same goes for Aron.</p></div></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2\cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The following $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$), denoting an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4\cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single line containing an integer: the number of integer pairs $(p, q)$ which make Aron <span class="tex-font-style-it">win</span>.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2\cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The following $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$), denoting an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4\cdot 10^5$. </p>

## Output

<p>For each test case, output a single line containing an integer: the number of integer pairs $(p, q)$ which make Aron <span class="tex-font-style-it">win</span>.</p>





```input1|2,3,9,10,11,12,13,14,15,16,17,18,19,20,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55
5
2
1 2
5
1 2
1 3
2 4
2 5
12
1 6
11 2
4 8
12 3
2 7
6 12
8 1
2 3
5 12
9 2
10 3
10
1 2
2 3
3 4
4 5
5 6
4 7
6 8
4 9
4 10
25
1 16
11 22
6 14
3 1
20 14
23 17
25 19
10 11
3 18
10 6
2 21
4 5
11 12
4 9
9 13
8 6
6 1
3 7
8 19
10 24
15 13
1 2
3 4
17 8
```




```output1
0
6
40
27
171
```



## Note

<p>In the first test case, all possible <span class="tex-font-style-it">caterpillars</span> are $(1, 2)$ and $(2, 1)$, resulting in a <span class="tex-font-style-it">tie</span> at the beginning, since both $p$ and $q$ are leaves.</p><p>In the second test case, the <span class="tex-font-style-it">caterpillars</span> that allow Aron to <span class="tex-font-style-it">win</span> are the following: $(1, 3)$, $(1, 4)$, $(1, 5)$, $(2, 3)$, $(2, 4)$, $(2, 5)$. Let's look at some specific <span class="tex-font-style-it">caterpillars</span>.</p><ul> <li> For the <span class="tex-font-style-it">caterpillar</span> $(1, 5)$: vertex $p = 1$ is not a leaf, but vertex $q = 5$ is, so Aron <span class="tex-font-style-it">wins</span> at the beginning. </li><li> For the <span class="tex-font-style-it">caterpillar</span> $(2, 1)$: vertex $p = 2$ is not a leaf, neither is vertex $q = 1$. In Nora's first move, she can choose to move the caterpillar towards vertex $5$, therefore the caterpillar becomes $(5, 2)$, and vertex $p = 5$ is a leaf, so Nora will <span class="tex-font-style-it">win</span>. </li></ul>
