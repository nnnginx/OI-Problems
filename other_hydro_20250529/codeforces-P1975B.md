## Description

<div><p>Mocha likes arrays, so before her departure, 378QAQ gave her an array $a$ consisting of $n$ positive integers as a gift.</p><p>Mocha thinks that $a$ is <span class="tex-font-style-it">beautiful</span> if there exist two numbers $i$ and $j$ ($1\leq i,j\leq n$, $i\neq j$) such that for all $k$ ($1 \leq k \leq n$), $a_k$ is divisible$^\dagger$ by either $a_i$ or $a_j$.</p><p>Determine whether $a$ is beautiful.</p><p>$^\dagger$ $x$ is divisible by $y$ if there exists an integer $z$ such that $x = y \cdot z$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3\leq n\leq 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i \leq 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if array $a$ is beautiful, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3\leq n\leq 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i \leq 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if array $a$ is beautiful, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7
4
3
7 3 8
5
7 1 9 3 5
5
4 12 2 6 3
5
7 49 9 3 1000000000
```




```output1
No
Yes
Yes
No
```



## Note

<p>In the first test case, any two numbers in the array are coprime, so the answer is "<span class="tex-font-style-tt">No</span>".</p><p>In the second test case, we can pick $i=2$ and $j=1$. Since every number in the array is divisible by $a_i = 1$, the answer is "<span class="tex-font-style-tt">Yes</span>".</p><p>In the third test case, we can pick $i=3$ and $j=5$. $2$ and $4$ is divisible by $a_i = 2$ while $3$, $6$ and $12$ is divisible by $a_j = 3$, so the answer is "<span class="tex-font-style-tt">Yes</span>".</p>
