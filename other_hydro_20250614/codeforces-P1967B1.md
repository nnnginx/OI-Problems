## Description

<div><p><span class="tex-font-style-bf">The two versions are different problems. You may want to read both versions. You can make hacks only if both versions are solved.</span></p><p>You are given two positive integers $n$, $m$.</p><p>Calculate the number of ordered pairs $(a, b)$ satisfying the following conditions:</p><ul> <li> $1\le a\le n$, $1\le b\le m$; </li><li> $a+b$ is a multiple of $b \cdot \gcd(a,b)$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($1\le n,m\le 2 \cdot 10^6$).</p><p>It is guaranteed that neither the sum of $n$ nor the sum of $m$ over all test cases exceeds $2 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, print a single integer: the number of valid pairs.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($1\le n,m\le 2 \cdot 10^6$).</p><p>It is guaranteed that neither the sum of $n$ nor the sum of $m$ over all test cases exceeds $2 \cdot 10^6$.</p>

## Output

<p>For each test case, print a single integer: the number of valid pairs.</p>





```input1|2,4,6
6
1 1
2 3
3 5
10 8
100 1233
1000000 1145141
```




```output1
1
3
4
14
153
1643498
```



## Note

<p>In the first test case, only $(1,1)$ satisfies the conditions.</p><p>In the fourth test case, $(1,1),(2,1),(2,2),(3,1),(4,1),(5,1),(6,1),(6,2),(6,3),(7,1),(8,1),(9,1),(10,1),(10,2)$ satisfy the conditions.</p>
