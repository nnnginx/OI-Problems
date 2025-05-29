## Description

<div><p>  </p><p>A permutation $p$ of length $n$$^{\text{∗}}$ is <span class="tex-font-style-it">perfect</span> if, for each index $i$ ($1 \le i \le n$), it satisfies the following:</p><ul> <li> The sum of the first $i$ elements $p_1 + p_2 + \ldots + p_i$ is <span class="tex-font-style-bf">not</span> a perfect square$^{\text{†}}$. </li></ul><p>You would like things to be perfect. Given a positive integer $n$, find a <span class="tex-font-style-it">perfect</span> permutation of length $n$, or print $-1$ if none exists.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). </p><p>$^{\text{†}}$A perfect square is an integer that is the square of an integer, e.g., $9=3^2$ is a perfect square, but $8$ and $14$ are not.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p></div><div class="output-specification"><p>For each test case:</p><ul> <li> If no solution exists, print a single integer $-1$. </li><li> Otherwise, print $n$ integers $p_1,p_2,\ldots,p_n$&nbsp;— the <span class="tex-font-style-it">perfect</span> permutation you find. </li></ul><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p>

## Output

<p>For each test case:</p><ul> <li> If no solution exists, print a single integer $-1$. </li><li> Otherwise, print $n$ integers $p_1,p_2,\ldots,p_n$&nbsp;— the <span class="tex-font-style-it">perfect</span> permutation you find. </li></ul><p>If there are multiple solutions, print any of them.</p>





```input1
3
1
4
5
```




```output1
-1
2 4 1 3
5 1 4 3 2
```



## Note

<p>In the first test case, there is only one permutation with length $n = 1$ that is $p = [1]$, which is not <span class="tex-font-style-it">perfect</span>:</p><ul> <li> $p_1 = 1 = x^2$ for $x = 1$. </li></ul><p>In the second test case, one possible <span class="tex-font-style-it">perfect</span> permutation with length $n = 4$ is $p = [2, 4, 1, 3]$:</p><ul> <li> $p_1 = 2 \neq x^2$; </li><li> $p_1 + p_2 = 2 + 4 = 6 \neq x^2$; </li><li> $p_1 + p_2 + p_3 = 2 + 4 + 1 = 7 \neq x^2$; </li><li> $p_1 + p_2 + p_3 + p_4 = 2 + 4 + 1 + 3 = 10 \neq x^2$. </li></ul><p>In the third test case, one possible <span class="tex-font-style-it">perfect</span> permutation with length $n = 5$ is $p = [5, 1, 4, 3, 2]$:</p><ul> <li> $p_1 = 5 \neq x^2$; </li><li> $p_1 + p_2 = 5 + 1 = 6 \neq x^2$; </li><li> $p_1 + p_2 + p_3 = 5 + 1 + 4 = 10 \neq x^2$; </li><li> $p_1 + p_2 + p_3 + p_4 = 5 + 1 + 4 + 3 = 13 \neq x^2$; </li><li> $p_1 + p_2 + p_3 + p_4 + p_5 = 5 + 1 + 4 + 3 + 2 = 15 \neq x^2$. </li></ul>
