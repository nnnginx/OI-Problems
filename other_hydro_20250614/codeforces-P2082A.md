## Description

<div><p>A matrix is called binary if all its elements are either $0$ or $1$.</p><p>Ecrade calls a binary matrix $A$ <span class="tex-font-style-it">good</span> if the following two properties hold:</p><ul> <li> The <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all numbers in each row of matrix $A$ is equal to $0$. </li><li> The <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all numbers in each column of matrix $A$ is equal to $0$. </li></ul><p>Ecrade has a binary matrix of size $n \cdot m$. He is interested in the minimum number of elements that need to be changed for the matrix to become <span class="tex-font-style-it">good</span>.</p><p>However, it seems a little difficult, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 400$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n, m$ ($1 \le n, m \le 100$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters consisting only of $0$ and $1$, describing the elements of Ecrade's matrix.</p><p>It is guaranteed that the sum of $n \cdot m$ across all test cases does not exceed $5 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, output a single integer, the minimum number of elements that need to be changed.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 400$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n, m$ ($1 \le n, m \le 100$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters consisting only of $0$ and $1$, describing the elements of Ecrade's matrix.</p><p>It is guaranteed that the sum of $n \cdot m$ across all test cases does not exceed $5 \cdot 10^4$.</p>

## Output

<p>For each test case, output a single integer, the minimum number of elements that need to be changed.</p>





```input1|2,3,4,5,10,11,12,13,18,19,20,21,24,25,26,27,28
7
3 3
010
101
010
3 3
000
000
000
3 3
100
010
001
3 3
101
010
000
3 3
000
010
000
1 4
0101
4 1
0
1
0
1
```




```output1
2
0
3
3
1
2
2
```



## Note

<p>In the first test case, he needs to change 2 elements to obtain the following matrix $\begin{pmatrix}1&amp;1&amp;0\\1&amp;0&amp;1\\0&amp;1&amp;1\end{pmatrix}$.</p><p>In the second test case, he can make no changes to obtain the following matrix $\begin{pmatrix}0&amp;0&amp;0\\0&amp;0&amp;0\\0&amp;0&amp;0\end{pmatrix}$.</p><p>In the third test case, he needs to change 3 elements to obtain the following matrix $\begin{pmatrix}1&amp;0&amp;1\\0&amp;0&amp;0\\1&amp;0&amp;1\end{pmatrix}$.</p>
