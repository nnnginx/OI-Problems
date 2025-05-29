## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/amalaofficial/mooo">MOOO! - Doja Cat</a></span></div><div class="epigraph-source">⠀</div></div><p>Farmer John has a permutation $p_1, p_2, \ldots, p_n$, where every integer from $0$ to $n-1$ occurs exactly once. He gives Bessie an array $a$ of length $n$ and challenges her to construct $p$ based on $a$. </p><p>The array $a$ is constructed so that $a_i$ = $\texttt{MEX}(p_1, p_2, \ldots, p_i) - p_i$, where the $\texttt{MEX}$ of an array is the minimum non-negative integer that does not appear in that array. For example, $\texttt{MEX}(1, 2, 3) = 0$ and $\texttt{MEX}(3, 1, 0) = 2$.</p><p>Help Bessie construct any valid permutation $p$ that satisfies $a$. The input is given in such a way that at least one valid $p$ exists. If there are multiple possible $p$, it is enough to print one of them.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the lengths of $p$ and $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-n \leq a_i \leq n$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that there is at least one valid $p$ for the given data.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers on a new line, the elements of $p$.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the lengths of $p$ and $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-n \leq a_i \leq n$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that there is at least one valid $p$ for the given data.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers on a new line, the elements of $p$.</p><p>If there are multiple solutions, print any of them.</p>





```input1|2,3,6,7
3
5
1 1 -2 1 2
5
1 1 1 1 1
3
-2 1 2
```




```output1
0 1 4 2 3 
0 1 2 3 4 
2 0 1
```



## Note

<p>In the first case, $p = [0, 1, 4, 2, 3]$ is one possible output.</p><p>$a$ will then be calculated as $a_1 = \texttt{MEX}(0) - 0 = 1$, $a_2 = \texttt{MEX}(0, 1) - 1 = 1$, $a_3 = \texttt{MEX}(0, 1, 4) - 4 = -2$, $a_4 = \texttt{MEX}(0, 1, 4, 2) - 2 = 1$, $a_5 = \texttt{MEX}(0, 1, 4, 2, 3) - 3 = 2$.</p><p>So, as required, $a$ will be $[1, 1, -2, 1, 2]$.</p>
