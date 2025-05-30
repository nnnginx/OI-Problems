## Description

<div><p>For the first place at the competition, Alex won many arrays of integers and was assured that these arrays are very expensive. After the award ceremony Alex decided to sell them. There is a rule in arrays pawnshop: you can sell array only if it can be compressed to a generator.</p><p>This generator takes four non-negative numbers $n$, $m$, $c$, $s$. $n$ and $m$ must be positive, $s$ non-negative and for $c$ it must be true that $0 \leq c &lt; m$. The array $a$ of length $n$ is created according to the following rules: </p><ul> <li> $a_1 = s \bmod m$, here $x \bmod y$ denotes remainder of the division of $x$ by $y$; </li><li> $a_i = (a_{i-1} + c) \bmod m$ for all $i$ such that $1 &lt; i \le n$. </li></ul><p>For example, if $n = 5$, $m = 7$, $c = 4$, and $s = 10$, then $a = [3, 0, 4, 1, 5]$.</p><p>Price of such an array is the value of $m$ in this generator.</p><p>Alex has a question: how much money he can get for each of the arrays. Please, help him to understand for every array whether there exist four numbers $n$, $m$, $c$, $s$ that generate this array. If yes, then maximize $m$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of arrays.</p><p>The first line of array description contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the size of this array.</p><p>The second line of array description contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$ )&nbsp;！ elements of the array. </p><p>It is guaranteed that the sum of array sizes does not exceed $10^5$.</p></div><div class="output-specification"><p>For every array print: </p><ul> <li> $-1$, if there are no such four numbers that generate this array; </li><li> $0$, if $m$ can be arbitrary large; </li><li> the maximum value $m$ and any appropriate $c$ ($0 \leq c &lt; m$) in other cases. </li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of arrays.</p><p>The first line of array description contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the size of this array.</p><p>The second line of array description contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$ )&nbsp;！ elements of the array. </p><p>It is guaranteed that the sum of array sizes does not exceed $10^5$.</p>

## Output

<p>For every array print: </p><ul> <li> $-1$, if there are no such four numbers that generate this array; </li><li> $0$, if $m$ can be arbitrary large; </li><li> the maximum value $m$ and any appropriate $c$ ($0 \leq c &lt; m$) in other cases. </li></ul>

## Samples

```input1
6
6
1 9 17 6 14 3
3
4 2 2
3
7 3 4
3
2 2 4
5
0 1000000000 0 1000000000 0
2
1 1
```

```output1
19 8
-1
-1
-1
2000000000 1000000000
0
```



