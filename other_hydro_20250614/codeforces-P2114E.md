## Description

<div><p>Once, Kirei stealthily infiltrated the trap-filled estate of the Ainzbern family but was discovered by Kiritugu's familiar. Assessing his strength, Kirei decided to retreat. The estate is represented as a tree with $n$ vertices, with the <span class="tex-font-style-bf">root</span> at vertex $1$. Each vertex of the tree has a number $a_i$ recorded, which represents the <span class="tex-font-style-it">danger</span> of vertex $i$. Recall that a tree is a connected undirected graph without cycles.</p><p>For a successful retreat, Kirei must compute the <span class="tex-font-style-it">threat</span> value for each vertex. The <span class="tex-font-style-it">threat</span> of a vertex is equal to the <span class="tex-font-style-bf">maximum</span> <span class="tex-font-style-it">alternating</span> sum along the vertical path starting from that vertex. The <span class="tex-font-style-it">alternating</span> sum along the vertical path starting from vertex $i$ is defined as $a_i - a_{p_i} + a_{p_{p_i}} - \ldots$, where $p_i$ is the parent of vertex $i$ on the path to the root (to vertex $1$).</p><p>For example, in the tree below, vertex $4$ has the following vertical paths: </p><ul> <li> $[4]$ with an alternating sum of $a_4 = 6$; </li><li> $[4, 3]$ with an alternating sum of $a_4 - a_3 = 6 - 2 = 4$; </li><li> $[4, 3, 2]$ with an alternating sum of $a_4 - a_3 + a_2 = 6 - 2 + 5 = 9$; </li><li> $[4, 3, 2, 1]$ with an alternating sum of $a_4 - a_3 + a_2 - a_1 = 6 - 2 + 5 - 4 = 5$. </li></ul><center> <img class="tex-graphics" src="./37536/file/8qFm6cy7.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The <span class="tex-font-style-it">dangers</span> of the vertices are indicated in red.</span> </center><p>Help Kirei compute the <span class="tex-font-style-it">threat</span> values for all vertices and escape the estate.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following describes the test cases.</p><p>The first line contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the <span class="tex-font-style-it">dangers</span> of the vertices.</p><p>The next $n - 1$ lines contain the numbers $v, u$ ($1 \le v, u \le n$, $v \neq u$)&nbsp;！ the description of the edges of the tree.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the given set of edges forms a tree.</p></div><div class="output-specification"><p>For each test case, output $n$ integers&nbsp;！ the <span class="tex-font-style-it">threat</span> of each vertex.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following describes the test cases.</p><p>The first line contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the <span class="tex-font-style-it">dangers</span> of the vertices.</p><p>The next $n - 1$ lines contain the numbers $v, u$ ($1 \le v, u \le n$, $v \neq u$)&nbsp;！ the description of the edges of the tree.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the given set of edges forms a tree.</p>

## Output

<p>For each test case, output $n$ integers&nbsp;！ the <span class="tex-font-style-it">threat</span> of each vertex.</p>





```input1|2,3,4,5,6,7
2
5
4 5 2 6 7
1 2
3 2
4 3
5 1
6
1000000000 500500500 900900900 9 404 800800800
3 4
5 1
2 5
1 6
6 4
```




```output1
4 5 2 9 7 
1000000000 1500500096 1701701691 199199209 404 800800800
```



## Note

<p>The tree from the first test case is depicted in the statement, and the maximum <span class="tex-font-style-it">variable-sign</span> sums are achieved as follows: </p><ol> <li> $a_1 = 4$; </li><li> $a_2 = 5$; </li><li> $a_3 = 2$; </li><li> $a_4 - a_3 + a_2 = 6 - 2 + 5 = 9$; </li><li> $a_5 = 7$. </li></ol>
