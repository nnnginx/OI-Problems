## Description

<div><p>Ecrade has an integer $x$. There are two kinds of operations.</p><ol> <li> Replace $x$ with $\left\lfloor \dfrac{x}{2}\right\rfloor$, where $\left\lfloor \dfrac{x}{2}\right\rfloor$ is the greatest integer $\le \dfrac{x}{2}$. </li><li> Replace $x$ with $\left\lceil \dfrac{x}{2}\right\rceil$, where $\left\lceil \dfrac{x}{2}\right\rceil$ is the smallest integer $\ge \dfrac{x}{2}$. </li></ol><p>Ecrade will perform exactly $n$ first operations and $m$ second operations in any order. He wants to know the minimum and the maximum possible value of $x$ after $n+m$ operations. However, it seems a little difficult, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains three integers $x$, $n$, and $m$ ($0 \le x, n, m \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print two integers in one line, representing the minimum and the maximum possible value of $x$ after $n + m$ operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains three integers $x$, $n$, and $m$ ($0 \le x, n, m \le 10^9$).</p>

## Output

<p>For each test case, print two integers in one line, representing the minimum and the maximum possible value of $x$ after $n + m$ operations.</p>





```input1|2,4,6
5
12 1 2
12 1 1
12 0 0
12 1000000000 1000000000
706636307 0 3
```




```output1
1 2
3 3
12 12
0 0
88329539 88329539
```



## Note

<p>For simplicity, we call the first operation $\text{OPER 1}$ and the second operation $\text{OPER 2}$.</p><p>In the first test case:</p><ul> <li> If we perform $12 \xrightarrow{\text{OPER 2}} 6 \xrightarrow{\text{OPER 2}} 3 \xrightarrow{\text{OPER 1}} 1$, we can obtain the minimum possible value $1$. </li><li> If we perform $12 \xrightarrow{\text{OPER 2}} 6 \xrightarrow{\text{OPER 1}} 3 \xrightarrow{\text{OPER 2}} 2$, we can obtain the maximum possible value $2$. </li></ul>
