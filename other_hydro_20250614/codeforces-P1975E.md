## Description

<div><p>You are given a tree of $n$ vertices numbered from $1$ to $n$. Initially, all vertices are colored white or black.</p><p>You are asked to perform $q$ queries:</p><ul> <li> "<span class="tex-font-style-tt">u</span>"&nbsp;¡ª toggle the color of vertex $u$ (if it was white, change it to black and vice versa). </li></ul><p>After each query, you should answer whether all the black vertices form a chain. That is, there exist two black vertices such that the simple path between them passes through all the black vertices and only the black vertices. Specifically, if there is only one black vertex, they form a chain. If there are no black vertices, they do <span class="tex-font-style-bf">not</span> form a chain.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1\leq n,q\leq 2\cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $c_1,c_2,\ldots,c_n$ ($c_i \in \{ \mathtt{0}, \mathtt{1} \}$)&nbsp;¡ª the initial color of the vertices. $c_i$ denotes the color of vertex $i$ where $\mathtt{0}$ denotes the color white, and $\mathtt{1}$ denotes the color black.</p><p>Then $n - 1$ lines follow, each line contains two integers $x_i$ and $y_i$ ($1 \le x_i,y_i \le n$), indicating an edge between vertices $x_i$ and $y_i$. It is guaranteed that these edges form a tree.</p><p>The following $q$ lines each contain an integer $u_i$ ($1 \le u_i \le n$), indicating the color of vertex $u_i$ needs to be toggled.</p><p>It is guaranteed that the sum of $n$ and $q$ over all test cases respectively does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each query, output "<span class="tex-font-style-tt">Yes</span>" if the black vertices form a chain, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1\leq n,q\leq 2\cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $c_1,c_2,\ldots,c_n$ ($c_i \in \{ \mathtt{0}, \mathtt{1} \}$)&nbsp;¡ª the initial color of the vertices. $c_i$ denotes the color of vertex $i$ where $\mathtt{0}$ denotes the color white, and $\mathtt{1}$ denotes the color black.</p><p>Then $n - 1$ lines follow, each line contains two integers $x_i$ and $y_i$ ($1 \le x_i,y_i \le n$), indicating an edge between vertices $x_i$ and $y_i$. It is guaranteed that these edges form a tree.</p><p>The following $q$ lines each contain an integer $u_i$ ($1 \le u_i \le n$), indicating the color of vertex $u_i$ needs to be toggled.</p><p>It is guaranteed that the sum of $n$ and $q$ over all test cases respectively does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each query, output "<span class="tex-font-style-tt">Yes</span>" if the black vertices form a chain, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p>





```input1|2,3,4,5
2
2 1
1 0
1 2
1
5 4
1 0 0 0 0
1 2
1 3
1 5
3 4
4
3
2
5
```




```input2|2,3,4,5,6,7,8,9,10,20,21,22
4
5 3
1 1 1 1 1
3 5
2 5
3 4
1 5
1
1
1
4 4
0 0 0 0
1 2
2 3
1 4
1
2
3
2
1 1
1
1
1 1
0
1
```




```output1
No
No
Yes
Yes
No
```




```output2
Yes
No
Yes
Yes
Yes
Yes
No
No
Yes
```



## Note

<p>In the second test case, the color of the vertices are as follows:</p><p>The initial tree: </p><center> <img class="tex-graphics" src="./34679/file/3EfWNMEX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The first query toggles the color of vertex $4$: </p><center> <img class="tex-graphics" src="./34679/file/kpGlUTpw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second query toggles the color of vertex $3$: </p><center> <img class="tex-graphics" src="./34679/file/ZyiyJcDG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The third query toggles the color of vertex $2$: </p><center> <img class="tex-graphics" src="./34679/file/issQlHqW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The fourth query toggles the color of vertex $5$: </p><center> <img class="tex-graphics" src="./34679/file/XvjpdJqG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
