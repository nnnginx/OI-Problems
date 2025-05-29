## Description

<div><p>You are given a forest of $k$ rooted trees$^{\text{∗}}$. Lumberjack Timofey wants to cut down the entire forest by applying the following operation: </p><ul> <li> Select a subtree$^{\text{†}}$ of any vertex of one of the trees and remove it from the tree. </li></ul><p>Timofey loves bitwise operations, so he wants the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of the sizes of the subtrees he removed to be maximum. Help him and find the maximum result he can obtain.</p><div class="statement-footnote"><p>$^{\text{∗}}$ A tree is a connected graph without cycles, loops, or multiple edges. In a rooted tree, a selected vertex is called a root. A forest is a collection of one or more trees.</p><p>$^{\text{†}}$ The subtree of a vertex $v$ is the set of vertices for which $v$ lies on the shortest path from this vertex to the root, including $v$ itself.</p></div></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains a single integer $k$ ($1 \leq k \leq 10^6$)&nbsp;— the number of trees in the forest.</p><p>This is followed by a description of each of the $k$ trees:</p><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the size of the tree. The vertices of the tree are numbered with integers from $1$ to $n$. The root of the tree is vertex number $1$.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots p_n$ ($1 \leq p_i &lt; i$), where $p_i$&nbsp;— the parent of vertex $i$.</p><p>It is guaranteed that the sum of $k$ and $n$ for all sets of input data does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the maximum result that can be obtained.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains a single integer $k$ ($1 \leq k \leq 10^6$)&nbsp;— the number of trees in the forest.</p><p>This is followed by a description of each of the $k$ trees:</p><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the size of the tree. The vertices of the tree are numbered with integers from $1$ to $n$. The root of the tree is vertex number $1$.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots p_n$ ($1 \leq p_i &lt; i$), where $p_i$&nbsp;— the parent of vertex $i$.</p><p>It is guaranteed that the sum of $k$ and $n$ for all sets of input data does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the maximum result that can be obtained.</p>





```input1|2,3,4,10,11,12
3
1
1
<br>
2
4
1 2 2
6
1 1 3 1 3
1
10
1 2 2 1 1 5 7 6 4
```




```output1
1
7
10
```



## Note

<p>In the second test case, the trees look like this:</p><p><img class="tex-graphics" src="./34816/file/Q5TCtbWF.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The first operation removes the entire second tree.</p><p><img class="tex-graphics" src="./34816/file/Rgc0QbIt.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The second operation removes vertex $4$ from the first tree.</p><p><img class="tex-graphics" src="./34816/file/yRaNTcNG.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The third operation removes the first tree. The result is $6|1|3 = 7$ ($|$ denotes bitwise OR).</p><p>In the third test case, the entire tree needs to be removed.</p>
