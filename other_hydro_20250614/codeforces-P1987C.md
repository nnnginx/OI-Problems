## Description

<div><p>There are $n$ flowers in a row, the $i$-th of them initially has a positive height of $h_i$ meters.</p><p>Every second, the wind will blow from the left, causing the height of some flowers to decrease.</p><p>Specifically, every second, for each $i$ from $1$ to $n$, in this order, the following happens: </p><ul> <li> If $i = n$ or $h_i &gt; h_{i + 1}$, the value of $h_i$ changes to $\max(0, h_i - 1)$. </li></ul><p>How many seconds will pass before $h_i=0$ for all $1 \le i \le n$ for the first time?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of flowers.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le 10 ^ 9$)&nbsp;！ the heights of the flowers.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of seconds that will pass before $h_i=0$ for all $1 \le i \le n$. </p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of flowers.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le 10 ^ 9$)&nbsp;！ the heights of the flowers.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of seconds that will pass before $h_i=0$ for all $1 \le i \le n$. </p>





```input1|2,3,6,7
4
3
1 1 2
2
3 1
1
9
5
7 4 4 3 2
```




```output1
4
3
9
7
```



## Note

<p>In the first test case, the flower heights change as follows: $[1, 1, 2] \rightarrow [1, 1, 1] \rightarrow [1, 1, 0] \rightarrow [1, 0, 0] \rightarrow [0, 0, 0]$.</p><p>In the second test case, the flower heights change as follows: $[3, 1] \rightarrow [2, 0] \rightarrow [1, 0] \rightarrow [0, 0]$.</p>
