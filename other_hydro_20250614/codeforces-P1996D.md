## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Counting is Fun!</span></div><div class="epigraph-source">！ satyam343</div></div><p>Given two integers $n$ and $x$, find the number of triplets ($a,b,c$) of <span class="tex-font-style-bf">positive integers</span> such that $ab + ac + bc \le n$ and $a + b + c \le x$. </p><p>Note that order matters (e.g. ($1, 1, 2$) and ($1, 2, 1$) are treated as different) and $a$, $b$, $c$ must be strictly greater than $0$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;！ the number of test cases.</p><p>Each test case contains two integers $n$ and $x$ ($1 \leq n,x \leq 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ and that the sum of $x$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>Output a single integer ！ the number of triplets ($a,b,c$) of positive integers such that $ab + ac + bc \le n$ and $a + b + c \le x$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;！ the number of test cases.</p><p>Each test case contains two integers $n$ and $x$ ($1 \leq n,x \leq 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ and that the sum of $x$ over all test cases does not exceed $10^6$.</p>

## Output

<p>Output a single integer ！ the number of triplets ($a,b,c$) of positive integers such that $ab + ac + bc \le n$ and $a + b + c \le x$.</p>





```input1|2,4
4
7 4
10 5
7 1000
900000 400000
```




```output1
4
10
7
1768016938
```



## Note

<p>In the first test case, the triplets are ($1, 1, 1$), ($1, 1, 2$), ($1, 2, 1$), and ($2, 1, 1$).</p><p>In the second test case, the triplets are ($1, 1, 1$), ($1, 1, 2$), ($1, 1, 3$), ($1, 2, 1$), ($1, 2, 2$), ($1, 3, 1$), ($2, 1, 1$), ($2, 1, 2$), ($2, 2, 1$), and ($3, 1, 1$).</p>
