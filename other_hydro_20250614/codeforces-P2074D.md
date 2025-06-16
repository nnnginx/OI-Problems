## Description

<div><p>The pink soldiers drew $n$ circles with their center <span class="tex-font-style-bf">on the $x$-axis</span> of the plane. Also, they have told that <span class="tex-font-style-bf">the sum of radii is exactly $m$</span>$^{\text{∗}}$.</p><p>Please find the number of integer points <span class="tex-font-style-bf">inside or on the border of</span> at least one circle. Formally, the problem is defined as follows.</p><p>You are given an integer sequence $x_1,x_2,\ldots,x_n$ and a positive integer sequence $r_1,r_2,\ldots,r_n$, where it is known that $\sum_{i=1}^n r_i = m$.</p><p>You must count the number of integer pairs $(x,y)$ that satisfy the following condition.</p><ul> <li> There exists an index $i$ such that $(x-x_i)^2 + y^2 \le r_i^2$ ($1 \le i \le n$). </li></ul><div class="statement-footnote"><p>$^{\text{∗}}$Is this information really useful? Don't ask me; I don't really know.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 2\cdot 10^5$).</p><p>The second line of each test case contains $x_1,x_2,\ldots,x_n$&nbsp;— the centers of the circles ($-10^9 \le x_i \le 10^9$).</p><p>The third line of each test case contains $r_1,r_2,\ldots,r_n$&nbsp;— the radii of the circles ($1 \le r_i$, $\sum_{i=1}^n r_i = m$).</p><p>It is guaranteed that <span class="tex-font-style-bf">the sum of $m$ over all test cases</span> does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the number of integer points satisfying the condition on a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 2\cdot 10^5$).</p><p>The second line of each test case contains $x_1,x_2,\ldots,x_n$&nbsp;— the centers of the circles ($-10^9 \le x_i \le 10^9$).</p><p>The third line of each test case contains $r_1,r_2,\ldots,r_n$&nbsp;— the radii of the circles ($1 \le r_i$, $\sum_{i=1}^n r_i = m$).</p><p>It is guaranteed that <span class="tex-font-style-bf">the sum of $m$ over all test cases</span> does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output the number of integer points satisfying the condition on a separate line.</p>





```input1|2,3,4,8,9,10
4
2 3
0 0
1 2
2 3
0 2
1 2
3 3
0 2 5
1 1 1
4 8
0 5 10 15
2 2 2 2
```




```output1
13
16
14
52
```



## Note

<p>On the first test case, the circle with $r_1=1$ is completely inside the circle with $r_2=2$. Therefore, you only have to count the number of integer points inside the latter. There are $13$ integer points such that $x^2+y^2 \le 2^2$, so the answer is $13$.</p><p>On the second test case, the circle with $r_1=1$ is not completely inside the circle with $r_2=2$. There are $3$ additional points that are inside the first circle but not inside the second circle, so the answer is $3+13=16$.</p>
