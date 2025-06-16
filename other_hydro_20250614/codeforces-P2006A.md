## Description

<div><p>Iris has a tree rooted at vertex $1$. Each vertex has a value of $\mathtt 0$ or $\mathtt 1$.</p><p>Let's consider a leaf of the tree (the vertex $1$ is never considered a leaf) and define its <span class="tex-font-style-it">weight</span>. Construct a string formed by the values of the vertices on the path starting at the root and ending in this leaf. Then the weight of the leaf is the difference between the number of occurrences of $\mathtt{10}$ and $\mathtt{01}$ substrings in it.</p><p>Take the following tree as an example. Green vertices have a value of $\mathtt 1$ while white vertices have a value of $\mathtt 0$.</p><center> <img class="tex-graphics" src="./34893/file/SWhVg5nF.png" style="max-width: 100.0%;max-height: 100.0%;">  </center><ul><li> Let's calculate the weight of the leaf $5$: the formed string is $\mathtt{10110}$. The number of occurrences of substring $\mathtt{10}$ is $2$, the number of occurrences of substring $\mathtt{01}$ is $1$, so the difference is $2 - 1 = 1$.</li><li> Let's calculate the weight of the leaf $6$: the formed string is $\mathtt{101}$. The number of occurrences of substring $\mathtt{10}$ is $1$, the number of occurrences of substring $\mathtt{01}$ is $1$, so the difference is $1 - 1 = 0$.</li></ul><p>The <span class="tex-font-style-it">score</span> of a tree is defined as the number of leaves with non-zero weight in the tree.</p><p>But the values of some vertices haven't been decided and will be given to you as $\texttt{?}$. Filling the blanks would be so boring, so Iris is going to invite Dora to play a game. On each turn, one of the girls chooses any of the remaining vertices with value $\texttt{?}$ and changes its value to $\mathtt{0}$ or $\mathtt{1}$, <span class="tex-font-style-bf">with Iris going first</span>. The game continues until there are no vertices with value $\mathtt{?}$ left in the tree. Iris aims to maximize the score of the tree, while Dora aims to minimize that.</p><p>Assuming that both girls play optimally, please determine the final score of the tree.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 5\cdot 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The following $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$)&nbsp;！ denoting an edge between vertices $u$ and $v$.</p><p>It's guaranteed that the given edges form a tree.</p><p>The last line contains a string $s$ of length $n$. The $i$-th character of $s$ represents the value of vertex $i$. It's guaranteed that $s$ only contains characters $\mathtt{0}$, $\mathtt{1}$ and $\mathtt{?}$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the final score of the tree.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 5\cdot 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The following $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$)&nbsp;！ denoting an edge between vertices $u$ and $v$.</p><p>It's guaranteed that the given edges form a tree.</p><p>The last line contains a string $s$ of length $n$. The $i$-th character of $s$ represents the value of vertex $i$. It's guaranteed that $s$ only contains characters $\mathtt{0}$, $\mathtt{1}$ and $\mathtt{?}$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer ！ the final score of the tree.</p>





```input1|2,3,4,5,6,12,13,14,15,16,17,25,26,27,28,29,30
6
4
1 2
1 3
4 1
0101
4
1 2
3 2
2 4
???0
5
1 2
1 3
2 4
2 5
?1?01
6
1 2
2 3
3 4
5 3
3 6
?0????
5
1 2
1 3
1 4
1 5
11?1?
2
2 1
??
```




```output1
2
1
1
2
1
0
```



## Note

<p>In the first test case, all the values of the vertices have been determined. There are three different paths from the root to a leaf:</p><ul> <li> From vertex $1$ to vertex $2$. The string formed by the path is $\mathtt{01}$, so the weight of the leaf is $0-1=-1$. </li><li> From vertex $1$ to vertex $3$. The string formed by the path is $\mathtt{00}$, so the weight of the leaf is $0-0=0$. </li><li> From vertex $1$ to vertex $4$. The string formed by the path is $\mathtt{01}$, so the weight of the leaf is $0-1=-1$. </li></ul><p>Thus, there are two leaves with non-zero weight, so the score of the tree is $2$.</p><p>In the second test case, one of the sequences of optimal choices for the two players can be:</p><ul> <li> Iris chooses to change the value of the vertex $3$ to $\mathtt 1$. </li><li> Dora chooses to change the value of the vertex $1$ to $\mathtt 0$. </li><li> Iris chooses to change the value of the vertex $2$ to $\mathtt 0$. </li></ul><p>The final tree is as follows:</p><center> <img class="tex-graphics" src="./34893/file/K1Ih1w75.png" style="max-width: 100.0%;max-height: 100.0%;">  </center><p>The only leaf with non-zero weight is $3$, so the score of the tree is $1$. Note that this may not be the only sequence of optimal choices for Iris and Dora.</p>
