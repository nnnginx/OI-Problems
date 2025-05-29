## Description

<div><p>A matrix is called quaternary if all its elements are $0$, $1$, $2$, or $3$.</p><p>Ecrade calls a quaternary matrix $A$ <span class="tex-font-style-it">good</span> if the following two properties hold.</p><ul> <li> The <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all numbers in each row of matrix $A$ is equal to $0$. </li><li> The <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all numbers in each column of matrix $A$ is equal to $0$. </li></ul><p>Ecrade has a quaternary matrix of size $n \times m$. He is interested in the minimum number of elements that need to be changed for the matrix to become <span class="tex-font-style-it">good</span>, and he also wants to find one of the possible resulting matrices.</p><p>However, it seems a little difficult, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^3$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters and consisting only of $0$, $1$, $2$, and $3$, describing the elements of Ecrade's matrix.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print the minimum number of elements that need to be changed for the matrix to become <span class="tex-font-style-it">good</span> on the first line, then print $n$ lines, each containing exactly $m$ characters and consisting only of $0$, $1$, $2$, and $3$, describing one of the possible resulting matrices.</p><p>If there are multiple possible resulting matrices, output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^3$).</p><p>This is followed by $n$ lines, each containing exactly $m$ characters and consisting only of $0$, $1$, $2$, and $3$, describing the elements of Ecrade's matrix.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print the minimum number of elements that need to be changed for the matrix to become <span class="tex-font-style-it">good</span> on the first line, then print $n$ lines, each containing exactly $m$ characters and consisting only of $0$, $1$, $2$, and $3$, describing one of the possible resulting matrices.</p><p>If there are multiple possible resulting matrices, output any of them.</p>





```input1|2,3,4,5,10,11,12,13,14,20,21,22,23,24
5
3 3
313
121
313
3 3
000
000
000
4 4
0123
1230
2301
3012
4 4
1232
2110
3122
1311
4 4
1232
2110
3122
1312
```




```output1
3
213
101
312
0
000
000
000
0
0123
1230
2301
3012
6
0132
2310
3131
1313
5
0132
2310
3120
1302
```


