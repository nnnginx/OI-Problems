## Description

<div><p>In 2077, everything became fashionable among robots, even arrays...</p><p>We will call an array of integers $a$ <span class="tex-font-style-it">fashionable</span> if $\min(a) + \max(a)$ is divisible by $2$ without a remainder, where $\min(a)$&nbsp;！ the value of the minimum element of the array $a$, and $\max(a)$&nbsp;！ the value of the maximum element of the array $a$.</p><p>You are given an array of integers $a_1, a_2, \ldots, a_n$. In one operation, you can remove any element from this array. Your task is to determine the minimum number of operations required to make the array $a$ <span class="tex-font-style-it">fashionable</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 50$)&nbsp;！ the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$)&nbsp;！ the elements of the array $a$.</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;！ the minimum number of operations required to make the array $a$ <span class="tex-font-style-it">fashionable</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 50$)&nbsp;！ the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$)&nbsp;！ the elements of the array $a$.</p>

## Output

<p>For each test case, output one integer&nbsp;！ the minimum number of operations required to make the array $a$ <span class="tex-font-style-it">fashionable</span>.</p>





```input1|2,3,6,7,10,11
6
2
5 2
7
3 1 4 1 5 9 2
7
2 7 4 6 9 11 5
3
1 2 1
2
2 1
8
8 6 3 6 4 1 1 6
```




```output1
1
0
2
1
1
3
```



## Note

<p>In the first test case, at least one element needs to be removed since $\min(a)+\max(a)=2+5=7$, and $7$ is not divisible by $2$. If any of the elements are removed, only one element will remain. Then $\max(a) + \min(a)$ will be divisible by $2$.</p><p>In the second test case, nothing needs to be removed since $\min(a)+\max(a)=1+9=10$, and $10$ is divisible by $2$.</p><p>In the third test case, you can remove the elements with values $2$ and $4$, then $\min(a)+\max(a)=5+11=16$, and $16$ is divisible by $2$.</p>
