## Description

<div><p>Boneca Ambalabu gives you a sequence of $n$ integers $a_1,a_2,\ldots,a_n$.</p><p>Output the maximum value of $(a_k\oplus a_1)+(a_k\oplus a_2)+\ldots+(a_k\oplus a_n)$ among all $1 \leq k \leq n$. Note that $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;每 the number of independent test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n\leq 2\cdot 10^5$)&nbsp;每 the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0 \leq a_i &lt; 2^{30}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum value on a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;每 the number of independent test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n\leq 2\cdot 10^5$)&nbsp;每 the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0 \leq a_i &lt; 2^{30}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum value on a new line.</p>





```input1|2,3,6,7,10,11
5
3
18 18 18
5
1 2 4 8 16
5
8 13 4 5 15
6
625 676 729 784 841 900
1
1
```




```output1
0
79
37
1555
0
```



## Note

<p>In the first test case, the best we can do is $(18\oplus18)+(18\oplus18)+(18\oplus18)=0$.</p><p>In the second test case, we choose $k=5$ to get $(16\oplus1)+(16\oplus2)+(16\oplus4)+(16\oplus8)+(16\oplus16)=79$.</p>
