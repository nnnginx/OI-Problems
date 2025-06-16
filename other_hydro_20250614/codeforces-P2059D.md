## Description

<div><p>You are given two connected undirected graphs with the same number of vertices. In both graphs, there is a token located at some vertex. In the first graph, the token is initially at vertex $s_1$, and in the second graph, the token is initially at vertex $s_2$. The following operation is repeated an <span class="tex-font-style-bf">infinite</span> number of times:</p><ul> <li> Let the token currently be at vertex $v_1$ in the first graph and at vertex $v_2$ in the second graph. </li><li> A vertex $u_1$, adjacent to $v_1$, is chosen in the first graph. </li><li> A vertex $u_2$, adjacent to $v_2$, is chosen in the second graph. </li><li> The tokens are moved to the chosen vertices: in the first graph, the token moves from $v_1$ to $u_1$, and in the second graph, from $v_2$ to $u_2$. </li><li> The cost of such an operation is equal to $|u_1 - u_2|$. </li></ul><p>Determine the minimum possible total cost of all operations or report that this value will be infinitely large.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $s_1$, and $s_2$ ($2 \le n \le 1000$, $1 \le s_1, s_2 \le n$)&nbsp;！ the number of vertices in each graph, the number of the vertex in the first graph where the token is initially located, and the number of the vertex in the second graph where the token is initially located.</p><p>The second line of each test case contains one integer $m_1$ ($1 \le m_1 \le 1000$)&nbsp;！ the number of edges in the first graph.</p><p>The $i$-th of the following $m_1$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$)&nbsp;！ the numbers of the endpoints of the $i$-th edge in the first graph.</p><p>The next line of each test case contains one integer $m_2$ ($1 \le m_2 \le 1000$)&nbsp;！ the number of edges in the second graph.</p><p>The $j$-th of the following $m_2$ lines contains two integers $c_j$ and $d_j$ ($1 \le c_j, d_j \le n$, $c_j \ne d_j$)&nbsp;！ the numbers of the endpoints of the $j$-th edge in the second graph.</p><p>It is guaranteed that the sum of $n$, the sum of $m_1$, and the sum of $m_2$ over all test cases do not exceed $1000$.</p><p>It is guaranteed that both graphs are connected.</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;！ the minimum total cost of all operations or $-1$, if this value will be infinitely large.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $s_1$, and $s_2$ ($2 \le n \le 1000$, $1 \le s_1, s_2 \le n$)&nbsp;！ the number of vertices in each graph, the number of the vertex in the first graph where the token is initially located, and the number of the vertex in the second graph where the token is initially located.</p><p>The second line of each test case contains one integer $m_1$ ($1 \le m_1 \le 1000$)&nbsp;！ the number of edges in the first graph.</p><p>The $i$-th of the following $m_1$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$)&nbsp;！ the numbers of the endpoints of the $i$-th edge in the first graph.</p><p>The next line of each test case contains one integer $m_2$ ($1 \le m_2 \le 1000$)&nbsp;！ the number of edges in the second graph.</p><p>The $j$-th of the following $m_2$ lines contains two integers $c_j$ and $d_j$ ($1 \le c_j, d_j \le n$, $c_j \ne d_j$)&nbsp;！ the numbers of the endpoints of the $j$-th edge in the second graph.</p><p>It is guaranteed that the sum of $n$, the sum of $m_1$, and the sum of $m_2$ over all test cases do not exceed $1000$.</p><p>It is guaranteed that both graphs are connected.</p>

## Output

<p>For each test case, output one integer&nbsp;！ the minimum total cost of all operations or $-1$, if this value will be infinitely large.</p>





```input1|2,3,4,5,6,7,8,9,10,11,12,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39
3
4 1 1
4
1 2
2 3
3 4
4 1
4
1 2
2 3
3 4
4 1
4 1 2
4
1 2
2 3
3 4
4 1
4
1 2
2 3
3 4
4 1
7 7 2
7
1 6
2 1
3 2
3 4
5 1
7 3
7 5
6
5 1
5 6
5 7
6 3
7 2
7 4
```




```output1
0
-1
7
```



## Note

<p>In the first test case, an infinite sequence of transitions can be constructed to the vertices $2, 3, 4, 1, 2, 3, 4, 1, \ldots$, along which the token can move in both the first and the second graphs.</p><p>In the second test case, it can be proven that the cost of any operation will be greater than $0$; therefore, the total cost of all operations will be infinitely large.</p>
