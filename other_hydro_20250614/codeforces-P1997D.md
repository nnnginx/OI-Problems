## Description

<div><p>You are given a rooted tree, consisting of $n$ vertices. The vertices in the tree are numbered from $1$ to $n$, and the root is the vertex $1$. The value $a_i$ is written at the $i$-th vertex.</p><p>You can perform the following operation any number of times (possibly zero): choose a vertex $v$ <span class="tex-font-style-bf">which has at least one child</span>; increase $a_v$ by $1$; and decrease $a_u$ by $1$ for all vertices $u$ that are in the subtree of $v$ (except $v$ itself). However, after each operation, the values on all vertices should be non-negative.</p><p>Your task is to calculate the maximum possible value written at the root using the aforementioned operation.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the initial values written at vertices.</p><p>The third line contains $n-1$ integers $p_2, p_3, \dots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the parent of the $i$-th vertex in the tree. Vertex $1$ is the root.</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the maximum possible value written at the root using the aforementioned operation.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the initial values written at vertices.</p><p>The third line contains $n-1$ integers $p_2, p_3, \dots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the parent of the $i$-th vertex in the tree. Vertex $1$ is the root.</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the maximum possible value written at the root using the aforementioned operation.</p>





```input1|2,3,4,8,9,10
3
4
0 1 0 2
1 1 3
2
3 0
1
5
2 5 3 9 6
3 1 5 2
```




```output1
1
3
6
```



## Note

<p>In the first test case, the following sequence of operations is possible:</p><ul> <li> perform the operation on $v=3$, then the values on the vertices will be $[0, 1, 1, 1]$; </li><li> perform the operation on $v=1$, then the values on the vertices will be $[1, 0, 0, 0]$. </li></ul>
