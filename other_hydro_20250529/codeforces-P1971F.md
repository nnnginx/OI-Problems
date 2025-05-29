## Description

<div><p>Given an integer $r$, find the number of lattice points that have a Euclidean distance from $(0, 0)$ <span class="tex-font-style-bf">greater than or equal to</span> $r$ but <span class="tex-font-style-bf">strictly less</span> than $r+1$.</p><p>A <span class="tex-font-style-it">lattice point</span> is a point with integer coordinates. The <span class="tex-font-style-it">Euclidean distance</span> from $(0, 0)$ to the point $(x,y)$ is $\sqrt{x^2 + y^2}$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single integer $r$ ($1 \leq r \leq 10^5$).</p><p>The sum of $r$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of lattice points that have an Euclidean distance $d$ from $(0, 0)$ such that $r \leq d &lt; r+1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single integer $r$ ($1 \leq r \leq 10^5$).</p><p>The sum of $r$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of lattice points that have an Euclidean distance $d$ from $(0, 0)$ such that $r \leq d &lt; r+1$.</p>





```input1|2,4,6
6
1
2
3
4
5
1984
```




```output1
8
16
20
24
40
12504
```



## Note

<p>The points for the first three test cases are shown below. </p><center> <img class="tex-graphics" src="./34657/file/I6NRZEfE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
