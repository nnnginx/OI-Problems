## Description

<div><p>There is an array of $5$ integers. Initially, you only know $a_1,a_2,a_4,a_5$. You may set $a_3$ to any positive integer, negative integer, or zero. The <span class="tex-font-style-it">Fibonacciness</span> of the array is the number of integers $i$ ($1 \leq i \leq 3$) such that $a_{i+2}=a_i+a_{i+1}$. Find the maximum <span class="tex-font-style-it">Fibonacciness</span> over all integer values of $a_3$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 500$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains four integers $a_1, a_2, a_4, a_5$ ($1 \leq a_i \leq 100$).</p></div><div class="output-specification"><p>For each test case, output the maximum <span class="tex-font-style-it">Fibonacciness</span> on a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 500$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains four integers $a_1, a_2, a_4, a_5$ ($1 \leq a_i \leq 100$).</p>

## Output

<p>For each test case, output the maximum <span class="tex-font-style-it">Fibonacciness</span> on a new line.</p>





```input1|2,4,6
6
1 1 3 5
1 3 2 1
8 10 28 100
100 1 100 1
1 100 1 100
100 100 100 100
```




```output1
3
2
2
1
1
2
```



## Note

<p>In the first test case, we can set $a_3$ to $2$ to achieve the maximal <span class="tex-font-style-it">Fibonacciness</span> of $3$.</p><p>In the third test case, it can be shown that $2$ is the maximum <span class="tex-font-style-it">Fibonacciness</span> that can be achieved. This can be done by setting $a_3$ to $18$.</p>
