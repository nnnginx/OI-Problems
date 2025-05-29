## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">If it was so, then let's make it a deal...</span></div><div class="epigraph-source">！ MayDay, <a href="https://www.youtube.com/watch?v=mtAc_bMYBsM&amp;list=PLj6NQzHFCvkHKIm0Vnk9LH3odqTIBRZ1Q&amp;index=15"><span class="tex-font-style-it">Gentleness</span></a></div></div><p><span class="tex-font-style-it">Even after copying the paintings from famous artists for ten years, unfortunately, Eric is still unable to become a skillful impressionist painter. He wants to forget something, but the white bear phenomenon just keeps hanging over him.</span></p><p>Eric still remembers $n$ pieces of impressions in the form of an integer array. He records them as $w_1, w_2, \ldots, w_n$. However, he has a poor memory of the impressions. For each $1 \leq i \leq n$, he can only remember that $l_i \leq w_i \leq r_i$.</p><p>Eric believes that impression $i$ is <span class="tex-font-style-it">unique</span> if and only if there exists a possible array $w_1, w_2, \ldots, w_n$ such that $w_i \neq w_j$ holds for all $1 \leq j \leq n$ with $j \neq i$.</p><p>Please help Eric determine whether impression $i$ is <span class="tex-font-style-it">unique</span> for every $1 \leq i \leq n$, <span class="tex-font-style-bf">independently</span> for each $i$. Perhaps your judgment can help rewrite the final story.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot 10^5$)&nbsp;！ the number of impressions.</p><p>Then $n$ lines follow, the $i$-th containing two integers $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq 2\cdot n$)&nbsp;！ the minimum possible value and the maximum possible value of $w_i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a binary string $s$ of length $n$: for each $1 \leq i \leq n$, if impression $i$ is <span class="tex-font-style-it">unique</span>, $s_i=\texttt{1}$; otherwise, $s_i=\texttt{0}$. Do <span class="tex-font-style-bf">not</span> output spaces.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot 10^5$)&nbsp;！ the number of impressions.</p><p>Then $n$ lines follow, the $i$-th containing two integers $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq 2\cdot n$)&nbsp;！ the minimum possible value and the maximum possible value of $w_i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a binary string $s$ of length $n$: for each $1 \leq i \leq n$, if impression $i$ is <span class="tex-font-style-it">unique</span>, $s_i=\texttt{1}$; otherwise, $s_i=\texttt{0}$. Do <span class="tex-font-style-bf">not</span> output spaces.</p>





```input1|2,3,4,10,11,12,13,14,15,16,25,26,27,28
5
2
1 1
1 1
4
1 3
1 3
1 3
1 3
6
3 6
2 2
1 2
1 1
3 4
2 2
7
3 4
4 4
4 4
1 3
2 5
1 4
2 2
3
4 5
4 4
5 5
```




```output1
00
1111
100110
1001111
011
```



## Note

<p>In the first test case, the only possible array $w$ is $[1, 1]$, making neither impression $1$ nor $2$ <span class="tex-font-style-it">unique</span> (since $w_1 = w_2$).</p><p>In the second test case, all impressions can be made <span class="tex-font-style-it">unique</span>:</p><ul> <li> For $i = 1$, we can set $w$ to $[1, 3, 2, 3]$, in which $w_1 \neq w_2$, $w_1 \neq w_3$, and $w_1 \neq w_4$; </li><li> For $i = 2$, we can set $w$ to $[2, 3, 1, 2]$, in which $w_2 \neq w_1$, $w_2 \neq w_3$, and $w_2 \neq w_4$; </li><li> For $i = 3$, we can set $w$ to $[1, 1, 3, 1]$; </li><li> For $i = 4$, we can set $w$ to $[2, 3, 3, 1]$. </li></ul><p>In the third test case, for $i = 4$, we can set $w$ to $[3, 2, 2, 1, 3, 2]$. Thus, impression $4$ is <span class="tex-font-style-it">unique</span>.</p>
