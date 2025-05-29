## Description

<div><p>Turtle gives you a string $s$, consisting of lowercase Latin letters.</p><p>Turtle considers a pair of integers $(i, j)$ ($1 \le i &lt; j \le n$) to be a <span class="tex-font-style-it">pleasant pair</span> if and only if there exists an integer $k$ such that $i \le k &lt; j$ and <span class="tex-font-style-bf">both</span> of the following two conditions hold:</p><ul> <li> $s_k \ne s_{k + 1}$; </li><li> $s_k \ne s_i$ <span class="tex-font-style-bf">or</span> $s_{k + 1} \ne s_j$. </li></ul><p>Besides, Turtle considers a pair of integers $(i, j)$ ($1 \le i &lt; j \le n$) to be a <span class="tex-font-style-it">good pair</span> if and only if $s_i = s_j$ <span class="tex-font-style-bf">or</span> $(i, j)$ is a pleasant pair.</p><p>Turtle wants to reorder the string $s$ so that the number of good pairs is <span class="tex-font-style-bf">maximized</span>. Please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ¡ª the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the string $s$ after reordering so that the number of good pairs is maximized. If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ¡ª the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the string $s$ after reordering so that the number of good pairs is maximized. If there are multiple answers, print any of them.</p>





```input1|2,3,6,7,10,11
5
3
abc
5
edddf
6
turtle
8
pppppppp
10
codeforces
```




```output1
acb
ddedf
urtlet
pppppppp
codeforces
```



## Note

<p>In the first test case, $(1, 3)$ is a good pair in the reordered string. It can be seen that we can't reorder the string so that the number of good pairs is greater than $1$. <span class="tex-font-style-tt">bac</span> and <span class="tex-font-style-tt">cab</span> can also be the answer.</p><p>In the second test case, $(1, 2)$, $(1, 4)$, $(1, 5)$, $(2, 4)$, $(2, 5)$, $(3, 5)$ are good pairs in the reordered string. <span class="tex-font-style-tt">efddd</span> can also be the answer.</p>
