## Description

<div><p> </p><p>You are given a tree with $n$ vertices, where each vertex can be colored red, blue, or white. The <span class="tex-font-style-it">coolness</span> of a coloring is defined as the maximum distance$^{\text{∗}}$ between a red and a blue vertex.</p><p>Formally, if we denote the color of the $i$-th vertex as $c_i$, the coolness of a coloring is $\max d(u, v)$ over all pairs of vertices $1\le u, v\le n$ where $c_u$ is <span class="tex-font-style-tt">red</span> and $c_v$ is <span class="tex-font-style-tt">blue</span>. If there are no red or no blue vertices, the coolness is zero.</p><p>Your task is to calculate the sum of coolness over all $3^n$ possible colorings of the tree, modulo $998\,244\,353$.</p><div class="statement-footnote"><p>$^{\text{∗}}$The distance between two vertices $a$ and $b$ in a tree is equal to the number of edges on the unique simple path between vertex $a$ and vertex $b$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 3000$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1\le u, v\le n$)&nbsp;— the endpoints of the edges of the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$. </p></div><div class="output-specification"><p>For each test case, output the sum of coolness over all $3^n$ possible colorings of the tree, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 3000$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1\le u, v\le n$)&nbsp;— the endpoints of the edges of the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$. </p>

## Output

<p>For each test case, output the sum of coolness over all $3^n$ possible colorings of the tree, modulo $998\,244\,353$.</p>





```input1|2,3,4,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27
3
3
1 2
2 3
6
1 2
1 3
1 4
3 5
5 6
17
1 2
1 3
1 4
1 5
2 6
2 7
2 8
3 9
3 10
7 11
7 12
11 13
13 14
14 15
10 16
16 17
```




```output1
18
1920
78555509
```



## Note

<p>In the first test case, there are $12$ colorings that have at least one blue and one red node. The following pictures show their coloring and their coolness:</p><center> <img class="tex-graphics" src="./37218/file/szKg0w9L.png" style="zoom: 150.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">All these colorings have coolness $2$</span> </center><center> <img class="tex-graphics" src="./37218/file/wsn5juwm.png" style="zoom: 150.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">All these colorings have coolness $1$</span> </center><p>Therefore, the sum of coolness over all possible colorings is $6\cdot 2 + 6\cdot 1 = 18$.</p><p>In the second test case, the following are some examples of colorings with a coolness of $3$:</p><center> <img class="tex-graphics" src="./37218/file/4uSlAt9R.png" style="zoom: 70.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small"></span> </center>
