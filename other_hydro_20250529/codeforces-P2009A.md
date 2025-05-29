## Description

<div><p>You are given two integers $a$ and $b$ ($a \leq b$). Over all possible integer values of $c$ ($a \leq c \leq b$), find the minimum value of $(c - a) + (b - c)$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 55$) ¡ª the number of test cases. </p><p>Each test case contains two integers $a$ and $b$ ($1 \leq a \leq b \leq 10$).</p></div><div class="output-specification"><p>For each test case, output the minimum possible value of $(c - a) + (b - c)$ on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 55$) ¡ª the number of test cases. </p><p>Each test case contains two integers $a$ and $b$ ($1 \leq a \leq b \leq 10$).</p>

## Output

<p>For each test case, output the minimum possible value of $(c - a) + (b - c)$ on a new line.</p>





```input1|2,4
3
1 2
3 10
5 5
```




```output1
1
7
0
```



## Note

<p>In the first test case, you can choose $c = 1$ and obtain an answer of $(1 - 1) + (2 - 1) = 1$. It can be shown this is the minimum value possible.</p><p>In the second test case, you can choose $c = 6$ and obtain an answer of $(6 - 3) + (10 - 6) = 7$. It can be shown this is the minimum value possible.</p>
