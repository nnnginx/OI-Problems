## Description

<div><p>Saturnita's mood depends on an array $a$ of length $n$, which only he knows the meaning of, and a function $f(k, a, l, r)$, which only he knows how to compute. Shown below is the pseudocode for his function $f(k, a, l, r)$. </p><pre class="lstlisting"><code class="prettyprint">function f(k, a, l, r):<br>   ans := 0<br>   for i from l to r (inclusive):<br>      while k is divisible by a[i]:<br>         k := k/a[i]<br>      ans := ans + k<br>   return ans<br></code></pre><p>You are given $q$ queries, each containing integers $k$, $l$, and $r$. For each query, please output $f(k,a,l,r)$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n \leq 10^5, 1 \leq q \leq 5\cdot 10^4$).</p><p>The following line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($2 \leq a_i \leq 10^5$).</p><p>The following $q$ lines each contain three integers $k$, $l$, and $r$ ($1 \leq k \leq 10^5, 1 \leq l \leq r \leq n$).</p><p>It is guaranteed that the sum of $n$ does not exceed $10^5$ over all test cases, and the sum of $q$ does not exceed $5\cdot 10^4$ over all test cases.</p></div><div class="output-specification"><p>For each query, output the answer on a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n \leq 10^5, 1 \leq q \leq 5\cdot 10^4$).</p><p>The following line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($2 \leq a_i \leq 10^5$).</p><p>The following $q$ lines each contain three integers $k$, $l$, and $r$ ($1 \leq k \leq 10^5, 1 \leq l \leq r \leq n$).</p><p>It is guaranteed that the sum of $n$ does not exceed $10^5$ over all test cases, and the sum of $q$ does not exceed $5\cdot 10^4$ over all test cases.</p>

## Output

<p>For each query, output the answer on a new line.</p>





```input1|2,3,4,5,6
2
5 3
2 3 5 7 11
2 1 5
2 2 4
2310 1 5
4 3
18 12 8 9
216 1 2
48 2 4
82944 1 4
```




```output1
5
6
1629
13
12
520
```


