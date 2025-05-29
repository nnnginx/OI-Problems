## Description

<div><p>Given an integer $n$, find an integer $x$ such that: </p><ul> <li> $2 \leq x \leq n$. </li><li> The sum of multiples of $x$ that are less than or equal to $n$ is maximized. Formally, $x + 2x + 3x + \dots + kx$ where $kx \leq n$ is maximized over all possible values of $x$. </li></ul></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 100$)&nbsp;¡ª the number of test cases.</p><p>Each test case contains a single integer $n$ ($2 \leq n \leq 100$).</p></div><div class="output-specification"><p>For each test case, output an integer, the optimal value of $x$. It can be shown there is only one unique answer.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 100$)&nbsp;¡ª the number of test cases.</p><p>Each test case contains a single integer $n$ ($2 \leq n \leq 100$).</p>

## Output

<p>For each test case, output an integer, the optimal value of $x$. It can be shown there is only one unique answer.</p>





```input1|2
2
3
15
```




```output1
3
2
```



## Note

<p>For $n = 3$, the possible values of $x$ are $2$ and $3$. The sum of all multiples of $2$ less than or equal to $n$ is just $2$, and the sum of all multiples of $3$ less than or equal to $n$ is $3$. Therefore, $3$ is the optimal value of $x$.</p><p>For $n = 15$, the optimal value of $x$ is $2$. The sum of all multiples of $2$ less than or equal to $n$ is $2 + 4 + 6 + 8 + 10 + 12 + 14 = 56$, which can be proven to be the maximal over all other possible values of $x$.</p>
