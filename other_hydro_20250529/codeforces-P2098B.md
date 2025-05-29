## Description

<div><p>Sasha wants to buy an apartment on a street where the houses are numbered from $1$ to $10^9$ from left to right.</p><p>There are $n$ bars on this street, located in houses with numbers $a_1, a_2, \ldots, a_n$. Note that there might be multiple bars in the same house, and in this case, these bars are considered distinct.</p><p>Sasha is afraid that by the time he buys the apartment, some bars may close, but <span class="tex-font-style-bf">no more than</span> $k$ bars can close.</p><p>For any house with number $x$, define $f(x)$ as the sum of $|x - y|$ over all open bars $y$ (that is, after closing some bars).</p><p>Sasha can potentially buy an apartment in a house with number $x$ (where $1 \le x \le 10^9$) if and only if it is possible to close at most $k$ bars so that after that $f(x)$ becomes minimal among all houses.</p><p>Determine how many different houses Sasha can potentially buy an apartment in.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 10^5, 0 \leq k &lt; n$)&nbsp;！ the number of bars and the maximum number of bars that can close.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the house numbers where the bars are located.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of houses where Sasha can buy an apartment.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 10^5, 0 \leq k &lt; n$)&nbsp;！ the number of bars and the maximum number of bars that can close.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the house numbers where the bars are located.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of houses where Sasha can buy an apartment.</p>





```input1|2,3,6,7
4
4 0
1 2 3 4
5 2
7 6 6 7 1
3 1
6 7 9
6 2
5 1 9 10 13 2
```




```output1
2
2
4
9
```



## Note

<p>In the first test case, none of the bars can close, so only houses numbered $2$ and $3$ are suitable. For the house numbered $2$, the sum of distances is $|2 - 1| + |2 - 2| + |2 - 3| + |2 - 4| = 4$, and for the house numbered $3$, the sum of distances is $|3 - 1| + |3 - 2| + |3 - 3| + |3 - 4| = 4$. However, for the house numbered $1$, the sum of distances will be $|1 - 1| + |1 - 2| + |1 - 3| + |1 - 4| = 6$, so the house numbered $1$ is not suitable. It can also be proven that Sasha cannot buy apartments in other houses.</p><p>In the second test case, the suitable houses are numbered $6$ and $7$. For Sasha to choose the house numbered $6$, it is sufficient that none of the bars close. For Sasha to choose the house numbered $7$, the bars in houses $1$ and $6$ can close. Then the bars will be located in houses numbered $6$, $7$, and $7$.</p>
