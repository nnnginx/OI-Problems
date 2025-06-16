## Description

<div><p>Let $D(n)$ represent the sum of digits of $n$. For how many integers $n$ where $10^{l} \leq n &lt; 10^{r}$ satisfy $D(k \cdot n) = k \cdot D(n)$? Output the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¨C the number of test cases. </p><p>Each test case contains three integers $l$, $r$, and $k$ ($0 \leq l &lt; r \leq 10^9$, $1 \leq k \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, output an integer, the answer, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¨C the number of test cases. </p><p>Each test case contains three integers $l$, $r$, and $k$ ($0 \leq l &lt; r \leq 10^9$, $1 \leq k \leq 10^9$).</p>

## Output

<p>For each test case, output an integer, the answer, modulo $10^9 + 7$.</p>





```input1|2,4,6
6
0 1 4
0 2 7
1 2 1
1 2 3
582 74663 3
0 3 1
```




```output1
2
3
90
12
974995667
999
```



## Note

<p>For the first test case, the only values of $n$ that satisfy the condition are $1$ and $2$.</p><p>For the second test case, the only values of $n$ that satisfy the condition are $1$, $10$, and $11$.</p><p>For the third test case, all values of $n$ between $10$ inclusive and $100$ exclusive satisfy the condition.</p>
