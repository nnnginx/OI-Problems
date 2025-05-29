## Description

<div><p>On the board Ivy wrote down all integers from $l$ to $r$, inclusive.</p><p>In an operation, she does the following: </p><ul> <li> pick two numbers $x$ and $y$ on the board, erase them, and in their place write the numbers $3x$ and $\lfloor \frac{y}{3} \rfloor$. (Here $\lfloor \bullet \rfloor$ denotes rounding down to the nearest integer).</li></ul> <p>What is the minimum number of operations Ivy needs to make all numbers on the board equal $0$? We have a proof that this is always possible.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \leq l &lt; r \leq 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of operations needed to make all numbers on the board equal $0$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \leq l &lt; r \leq 2 \cdot 10^5$).</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of operations needed to make all numbers on the board equal $0$.</p>





```input1|2,4
4
1 3
2 4
199999 200000
19 84
```




```output1
5
6
36
263
```



## Note

<p>In the first test case, we can perform $5$ operations as follows: $$ 1,2,3 \xrightarrow[x=1,\,y=2]{} 3,0,3 \xrightarrow[x=0,\,y=3]{} 1,0,3 \xrightarrow[x=0,\,y=3]{} 1,0,1 \xrightarrow[x=0,\,y=1]{} 0,0,1 \xrightarrow[x=0,\,y=1]{} 0,0,0 .$$</p>
