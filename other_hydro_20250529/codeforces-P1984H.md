## Description

<div><p>There are $n$ towers at $n$ distinct points $(x_1, y_1), (x_2, y_2), \ldots, (x_n, y_n)$, such that no three are collinear and no four are concyclic. Initially, you own towers $(x_1, y_1)$ and $(x_2, y_2)$, and you want to capture all of them. To do this, you can do the following operation any number of times: </p><ul> <li> Pick two towers $P$ and $Q$ you own and one tower $R$ you don't own, such that the circle through $P$, $Q$, and $R$ contains <span class="tex-font-style-bf">all</span> $n$ towers inside of it. </li><li> Afterwards, capture all towers in or on triangle $\triangle PQR$, including $R$ itself. </li></ul> An <span class="tex-font-style-it">attack plan</span> is a series of choices of $R$ ($R_1, R_2, \ldots, R_k$) using the above operations after which you capture all towers. Note that two attack plans are considered different only if they differ in their choice of $R$ in some operation; in particular, two attack plans using the same choices of $R$ but different choices of $P$ and $Q$ are considered the same.<p>Count the number of attack plans of <span class="tex-font-style-bf">minimal length</span>. Note that it might not be possible to capture all towers, in which case the answer is $0$. </p><p>Since the answer may be large, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 250$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($4 \leq n \leq 100$)&nbsp;！ the number of towers.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($-10^4 \leq x_i, y_i \leq 10^4$)&nbsp;！ the location of the $i$-th tower. Initially, you own towers $(x_1, y_1)$ and $(x_2, y_2)$.</p><p>All towers are at distinct locations, no three towers are collinear, and no four towers are concyclic.</p><p>The sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of attack plans of minimal length after which you capture all towers, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 250$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($4 \leq n \leq 100$)&nbsp;！ the number of towers.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($-10^4 \leq x_i, y_i \leq 10^4$)&nbsp;！ the location of the $i$-th tower. Initially, you own towers $(x_1, y_1)$ and $(x_2, y_2)$.</p><p>All towers are at distinct locations, no three towers are collinear, and no four towers are concyclic.</p><p>The sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of attack plans of minimal length after which you capture all towers, modulo $998\,244\,353$.</p>





```input1|2,3,4,5,6,7,15,16,17,18,19,20,21,22
3
5
1 1
2 5
3 3
4 2
5 4
6
1 1
3 3
1 2
2 1
3 10000
19 84
7
2 7
-4 -3
-3 6
3 1
-5 2
1 -4
-1 7
```




```output1
1
0
10
```



## Note

<p>In the first test case, there is only one possible attack plan of shortest length, shown below.</p><center> <img class="tex-graphics" src="./34742/file/7lqm8fF4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ul> <li> Use the operation with $P =$ tower $1$, $Q =$ tower $2$, and $R =$ tower $5$. The circle through these three towers contains all towers inside of it, and as a result towers $3$ and $5$ are captured. </li><li> Use the operation with $P =$ tower $5$, $Q =$ tower $1$, and $R =$ tower $4$. The circle through these three towers contains all towers inside of it, and as a result tower $4$ is captured. </li></ul><p>In the second case, for example, you can never capture the tower at $(3, 10\,000)$.</p>
