## Description

<div><p> </p><p>The <span class="tex-font-style-it">distance</span> of a value $x$ in an array $c$, denoted as $d_x(c)$, is defined as the largest gap between any two occurrences of $x$ in $c$. </p><p>Formally, $d_x(c) = \max(j - i)$ over all pairs $i &lt; j$ where $c_i = c_j = x$. If $x$ appears only once or not at all in $c$, then $d_x(c) = 0$. </p><p>The <span class="tex-font-style-it">beauty</span> of an array is the sum of the distances of each distinct value in the array. Formally, the beauty of an array $c$ is equal to $\sum\limits_{1\le x\le n} d_x(c)$.</p><p>Given an array $a$ of length $n$, an array $b$ is <span class="tex-font-style-it">nice</span> if it also has length $n$ and its elements satisfy $1\le b_i\le a_i$ for all $1\le i\le n$. Your task is to find the maximum possible beauty of any nice array.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot10^5$)&nbsp;�� the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$)&nbsp;�� the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer representing the maximum possible beauty among all nice arrays.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot10^5$)&nbsp;�� the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$)&nbsp;�� the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$. </p>

## Output

<p>For each test case, output a single integer representing the maximum possible beauty among all nice arrays.</p>





```input1|2,3,6,7
4
4
1 2 1 2
2
2 2
10
1 2 1 5 1 2 2 1 1 2
8
1 5 2 8 4 1 4 2
```




```output1
4
1
16
16
```



## Note

<p>In the first test case, if $b = [1, 2, 1, 2]$, then $d_1(b) = 3 - 1 = 2$ and $d_2(b) = 4 - 2 = 2$, resulting in a beauty of $2 + 2 = 4$. It can be proven that there are no nice arrays with a beauty greater than $4$.</p><p>In the second test case, both $b = [1, 1]$ and $b = [2, 2]$ are valid solutions with a beauty of $1$.</p><p>In the third test case, if $b = [1, 2, 1, 4, 1, 2, 1, 1, 1, 2]$ with $d_1(b) = 9 - 1 = 8$, $d_2(b) = 10 - 2 = 8$, and $d_4(b) = 0$, resulting in a beauty of $16$.</p>
