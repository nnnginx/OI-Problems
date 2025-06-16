## Description

<div><p>You are given a binary (consisting only of <span class="tex-font-style-tt">0</span>s and <span class="tex-font-style-tt">1</span>s) $n \times m$ matrix. You are also given a XORificator, using which you can invert all the values in a chosen row (i.e. replace <span class="tex-font-style-tt">0</span> with <span class="tex-font-style-tt">1</span> and <span class="tex-font-style-tt">1</span> with <span class="tex-font-style-tt">0</span>).</p><p>A column in the matrix is considered <span class="tex-font-style-it">special</span> if it contains exactly one <span class="tex-font-style-tt">1</span>. Your task is to find the maximum number of columns that can be made <span class="tex-font-style-it">special</span> at the same time, and the set of rows the XORificator should be used on to achieve that.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 3 \cdot 10^5$, $n \cdot m \leq 3 \cdot 10^5$).</p><p>Each of the following $n$ lines of the test case contains a binary string of length $m$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two lines.</p><p>In the first line, output the maximum number of <span class="tex-font-style-it">special</span> columns that is possible to get simultaneously.</p><p>In the second line, output a binary string of length $n$, where the $i$-th character is <span class="tex-font-style-tt">0</span>, if you don't use the XORificator on the $i$-th row, and <span class="tex-font-style-tt">1</span>, if you use the XORificator on the $i$-th row.</p><p>If there are multiple valid XORificator configurations that achieve the optimal answer, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 3 \cdot 10^5$, $n \cdot m \leq 3 \cdot 10^5$).</p><p>Each of the following $n$ lines of the test case contains a binary string of length $m$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output two lines.</p><p>In the first line, output the maximum number of <span class="tex-font-style-it">special</span> columns that is possible to get simultaneously.</p><p>In the second line, output a binary string of length $n$, where the $i$-th character is <span class="tex-font-style-tt">0</span>, if you don't use the XORificator on the $i$-th row, and <span class="tex-font-style-tt">1</span>, if you use the XORificator on the $i$-th row.</p><p>If there are multiple valid XORificator configurations that achieve the optimal answer, you can output any of them.</p>





```input1|2,3,4,5,8,9,13,14,15,16
5
3 4
1010
0110
0100
1 1
1
1 1
0
2 5
00101
10110
3 3
101
111
000
```




```output1
3
010
1
0
1
1
3
00
2
010
```



## Note

<p>In the first test case, you can use the XORificator on the second row to make the columns $2$, $3$, and $4$ <span class="tex-font-style-it">special</span>.</p><p>In the second test case, the only column is already <span class="tex-font-style-it">special</span>, so you don't need to use the XORificator.</p>
