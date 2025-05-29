## Description

<div><p>Today, Cat and Fox found an array $a$ consisting of $n$ non-negative integers. </p><p>Define the <span class="tex-font-style-it">loneliness</span> of $a$ as the <span class="tex-font-style-bf">smallest</span> positive integer $k$ ($1 \le k \le n$) such that for any two positive integers $i$ and $j$ ($1 \leq i, j \leq n - k +1$), the following holds: $$a_i | a_{i+1} | \ldots | a_{i+k-1} = a_j | a_{j+1} | \ldots | a_{j+k-1},$$ where $x | y$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of $x$ and $y$. In other words, for every $k$ consecutive elements, their bitwise OR should be the same. Note that the loneliness of $a$ is well-defined, because for $k = n$ the condition is satisfied.</p><p>Cat and Fox want to know how lonely the array $a$ is. Help them calculate the loneliness of the found array.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4 $)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{20}$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer &nbsp;！ the loneliness of the given array.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4 $)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{20}$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print one integer &nbsp;！ the loneliness of the given array.</p>





```input1|2,3,6,7,10,11,14,15
7
1
0
3
2 2 2
3
1 0 2
5
3 0 1 4 2
5
2 0 4 0 2
7
0 0 0 0 1 2 4
8
0 1 3 2 2 1 0 3
```




```output1
1
1
3
4
4
7
3
```



## Note

<p>In the first example, the loneliness of an array with a single element is always $1$, so the answer is $1$. </p><p>In the second example, the OR of each subarray of length $k = 1$ is $2$, so the loneliness of the whole array is $1$.</p><p>In the seventh example, it's true that $(0 | 1 | 3) = (1 | 3 | 2) = (3 | 2 | 2) = (2 | 2 | 1) = (2 | 1 | 0) = (1 | 0 | 3) = 3$, so the condition is satisfied for $k = 3$. We can verify that the condition is not true for any smaller $k$, so the answer is indeed $3$.</p>
