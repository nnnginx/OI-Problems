## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Drink water.</span></div><div class="epigraph-source">！ Sun Tzu, <span class="tex-font-style-it">The Art of Becoming a Healthy Programmer</span></div></div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that $x=1$ in this version. You must solve both versions to be able to hack.</span></p><p>You are given two integers $n$ and $x$ ($x=1$). There are $n$ balls lined up in a row, numbered from $1$ to $n$ from left to right. Initially, there is a value $a_i$ written on the $i$-th ball.</p><p>For each integer $i$ from $1$ to $n$, we define a function $f(i)$ as follows: </p><ul> <li> Suppose you have a set $S = \{1, 2, \ldots, i\}$.<p> </p></li><li> In each operation, you have to select an integer $l$ ($1 \leq l &lt; i$) from $S$ such that $l$ is not the largest element of $S$. Suppose $r$ is the smallest element in $S$ which is greater than $l$.<p> </p><ul> <li> If $a_l &gt; a_r$, you set $a_l = a_l + a_r$ and remove $r$ from $S$. </li><li> If $a_l &lt; a_r$, you set $a_r = a_l + a_r$ and remove $l$ from $S$. </li><li> If $a_l = a_r$, you choose either the integer $l$ or $r$ to remove from $S$: <ul> <li> If you choose to remove $l$ from $S$, you set $a_r = a_l + a_r$ and remove $l$ from $S$. </li><li> If you choose to remove $r$ from $S$, you set $a_l = a_l + a_r$ and remove $r$ from $S$. </li></ul> </li></ul><p> </p></li><li> $f(i)$ denotes the number of integers $j$ ($1 \le j \le i$) such that it is possible to obtain $S = \{j\}$ after performing the above operations exactly $i - 1$ times. </li></ul><p>For each integer $i$ from $x$ to $n$, you need to find $f(i)$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \leq n \leq 2 \cdot 10^5; x = 1$)&nbsp;！ the number of balls and the smallest index $i$ for which you need to find $f(i)$.</p><p>The second line of each test case contains $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the initial number written on each ball.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n-x+1$ space separated integers on a new line, where the $j$-th integer should represent $f(x+j-1)$.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \leq n \leq 2 \cdot 10^5; x = 1$)&nbsp;！ the number of balls and the smallest index $i$ for which you need to find $f(i)$.</p><p>The second line of each test case contains $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the initial number written on each ball.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n-x+1$ space separated integers on a new line, where the $j$-th integer should represent $f(x+j-1)$.</p>





```input1|2,3,6,7
3
5 1
1 2 3 2 1
7 1
4 5 1 2 1 4 5
11 1
1 2 3 1 1 9 3 2 4 1 3
```




```output1
1 1 2 2 3
1 1 1 1 1 3 4
1 1 2 2 2 1 1 1 3 3 4
```



## Note

<p>In the first test case, below are the possible values of $j$ for each $f(i)$ from $1$ to $n$.</p><ul> <li> For $f(1)$, the only possible value of $j$ is $1$. </li><li> For $f(2)$, the only possible value of $j$ is $2$. </li><li> For $f(3)$, the possible values of $j$ are $2$ and $3$. </li><li> For $f(4)$, the possible values of $j$ are $2$ and $3$. </li><li> For $f(5)$, the possible values of $j$ are $2$, $3$, and $4$. </li></ul>
