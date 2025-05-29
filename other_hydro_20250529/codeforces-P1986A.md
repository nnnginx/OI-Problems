## Description

<div><p>You are given three points with integer coordinates $x_1$, $x_2$, and $x_3$ on the $X$ axis ($1 \leq x_i \leq 10$). You can choose any point with an integer coordinate $a$ on the $X$ axis. Note that the point $a$ may coincide with $x_1$, $x_2$, or $x_3$. Let $f(a)$ be the total distance from the given points to the point $a$. Find the smallest value of $f(a)$.</p><p>The distance between points $a$ and $b$ is equal to $|a - b|$. For example, the distance between points $a = 5$ and $b = 2$ is $3$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases. Then follows their descriptions.</p><p>The single line of each test case contains three integers $x_1$, $x_2$, and $x_3$ ($1 \leq x_i \leq 10$)&nbsp;！ the coordinates of the points.</p></div><div class="output-specification"><p>For each test case, output the smallest value of $f(a)$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases. Then follows their descriptions.</p><p>The single line of each test case contains three integers $x_1$, $x_2$, and $x_3$ ($1 \leq x_i \leq 10$)&nbsp;！ the coordinates of the points.</p>

## Output

<p>For each test case, output the smallest value of $f(a)$.</p>





```input1|2,4,6,8
8
1 1 1
1 5 9
8 2 8
10 9 3
2 1 1
2 4 1
7 3 5
1 9 4
```




```output1
0
8
6
7
1
3
4
8
```



## Note

<p>In the first test case, the smallest value of $f(a)$ is achieved when $a = 1$: $f(1) = |1 - 1| + |1 - 1| + |1 - 1| = 0$.</p><p>In the second test case, the smallest value of $f(a)$ is achieved when $a = 5$: $f(5) = |1 - 5| + |5 - 5| + |9 - 5| = 8$.</p><p>In the third test case, the smallest value of $f(a)$ is achieved when $a = 8$: $f(8) = |8 - 8| + |2 - 8| + |8 - 8| = 6$.</p><p>In the fourth test case, the smallest value of $f(a)$ is achieved when $a = 9$: $f(10) = |10 - 9| + |9 - 9| + |3 - 9| = 7$.</p>
