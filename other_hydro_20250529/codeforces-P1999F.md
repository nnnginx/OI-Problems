## Description

<div><p>Arul has a <span class="tex-font-style-bf">binary</span> array$^{\text{∗}}$ $a$ of length $n$.</p><p>He will take all subsequences$^{\text{†}}$ of length $k$ ($k$ is odd) of this array and find their median.$^{\text{‡}}$</p><p>What is the sum of all these values?</p><p>As this sum can be very large, output it modulo $10^9 + 7$. In other words, print the remainder of this sum when divided by $10^9 + 7$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A binary array is an array consisting only of zeros and ones.</p><p>$^{\text{†}}$An array $b$ is a subsequence of an array $a$ if $b$ can be obtained from $a$ by the deletion of several (possibly, zero or all) elements. Subsequences <span class="tex-font-style-bf">don't</span> have to be contiguous.</p><p>$^{\text{‡}}$The median of an array of odd length $k$ is the $\frac{k+1}{2}$-th element when sorted.</p></div></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, <span class="tex-font-style-bf">$k$ is odd</span>)&nbsp;— the length of the array and the length of the subsequence, respectively.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the sum modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, <span class="tex-font-style-bf">$k$ is odd</span>)&nbsp;— the length of the array and the length of the subsequence, respectively.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the sum modulo $10^9 + 7$.</p>





```input1|2,3,6,7,10,11,14,15
8
4 3
1 0 0 1
5 1
1 1 1 1 1
5 5
0 1 0 1 0
6 3
1 0 1 0 1 1
4 3
1 0 1 1
5 3
1 0 1 1 0
2 1
0 0
34 17
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
```




```output1
2
5
0
16
4
7
0
333606206
```



## Note

<p>In the first test case, there are four subsequences of $[1,0,0,1]$ with length $k=3$: </p><ul> <li> $[1,0,0]$: median $= 0$. </li><li> $[1,0,1]$: median $= 1$. </li><li> $[1,0,1]$: median $= 1$. </li><li> $[0,0,1]$: median $= 0$. </li></ul> The sum of the results is $0+1+1+0=2$.<p>In the second test case, all subsequences of length $1$ have median $1$, so the answer is $5$.</p>
