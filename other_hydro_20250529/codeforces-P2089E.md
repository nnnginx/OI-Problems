## Description

<div><p>The world of the black cat is collapsing. </p><p>In this world, which can be represented as a rooted tree with root at node $1$, Liki and Sasami need to uncover the truth about the world. </p><p>Each day, they can explore a node $u$ that has not yet collapsed. After this exploration, the black cat causes $u$ and all nodes in its subtree to collapse. Additionally, at the end of the $i$ th day, if it exists, the number $n-i+1$ node will also collapse. </p><p>For each $i$ from $1$ to $n$, determine the number of exploration schemes where Liki and Sasami explore exactly $i$ days (i.e., they perform exactly $i$ operations), with the last exploration being at node $1$. The result should be computed modulo $998\,244\,353$.</p><p><span class="tex-font-style-bf">Note:</span> It is guaranteed that nodes $1$ to $n$ can form a "DFS" order of the tree, meaning there exists a depth-first search traversal where the $i$ th visited node is $i$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains exactly one number $n$ ($3 \le n \le 80$).</p><p>Each of the following $n - 1$ lines contains two integers $u_i$ and $v_i$, representing two vertices connected by an edge ($1 \le u_i, v_i \le n$). It is guaranteed that the given edges form a tree. It is also guaranteed that the vertices can form a "DFS" traversal order.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $80$</p></div><div class="output-specification"><p>For each test case, print $n$ integers, where the $i$ th integer represents the number of exploration schemes for exactly $i$ days, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains exactly one number $n$ ($3 \le n \le 80$).</p><p>Each of the following $n - 1$ lines contains two integers $u_i$ and $v_i$, representing two vertices connected by an edge ($1 \le u_i, v_i \le n$). It is guaranteed that the given edges form a tree. It is also guaranteed that the vertices can form a "DFS" traversal order.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $80$</p>

## Output

<p>For each test case, print $n$ integers, where the $i$ th integer represents the number of exploration schemes for exactly $i$ days, modulo $998\,244\,353$.</p>





```input1|2,3,4,5
2
4
1 2
2 3
2 4
7
4 2
6 1
5 1
7 6
2 3
1 2
```




```output1
1 3 3 1
1 6 23 48 43 17 1
```



## Note

<p>For the first test case, the following operation sequences are legal:</p><p>$\{1\},\{2,1\},\{3,1\},\{4,1\},\{3,2,1\},\{4,2,1\},\{4,3,1\},\{4,3,2,1\}$.</p>
