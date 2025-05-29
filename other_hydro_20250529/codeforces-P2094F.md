## Description

<div><p>Trulicina gives you integers $n$, $m$, and $k$. It is guaranteed that $k\geq 2$ and $n\cdot m\equiv 0 \pmod{k}$.</p><p>Output a $n$ by $m$ grid of integers such that each of the following criteria hold:</p><ul> <li> Each integer in the grid is between $1$ and $k$, inclusive. </li><li> Each integer from $1$ to $k$ appears an equal number of times. </li><li> No two cells that share an edge have the same integer. </li></ul><p>It can be shown that such a grid always exists. If there are multiple solutions, output any.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \leq n\cdot m\leq 2\cdot 10^5, 2\leq k\leq n\cdot m, n\cdot m\equiv 0 \pmod{k})$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ lines, each containing $m$ integers that satisfy the criteria. If there are multiple solutions, output any.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \leq n\cdot m\leq 2\cdot 10^5, 2\leq k\leq n\cdot m, n\cdot m\equiv 0 \pmod{k})$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ lines, each containing $m$ integers that satisfy the criteria. If there are multiple solutions, output any.</p>





```input1|2,4
3
2 2 2
3 4 6
5 5 25
```




```output1
1 2
2 1
1 6 1 6
2 5 2 5
3 4 3 4
17 2 12 25 14
3 1 6 19 11
8 20 23 24 4
9 10 5 13 21
22 7 15 18 16
```


