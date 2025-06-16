## Description

<div><p>Gellyfish has an array of $n$ integers $c_1, c_2, \ldots, c_n$. In the beginning, $c = [a_1, a_2, \ldots, a_n]$.</p><p>Gellyfish will make $q$ modifications to $c$.</p><p>For $i = 1,2,\ldots,q$, Gellyfish is given three integers $x_i$, $y_i$, and $z_i$ between $1$ and $n$. Then Gellyfish will set $c_{z_i} := \min(c_{x_i}, c_{y_i})$.</p><p>After the $q$ modifications, $c = [b_1, b_2, \ldots, b_n]$.</p><p>Now Flower knows the value of $b$ and the value of the integers $x_i$, $y_i$, and $z_i$ for all $1 \leq i \leq q$, but she doesn't know the value of $a$.</p><p>Flower wants to find any possible value of the array $a$ or report that no such $a$ exists.</p><p>If there are multiple possible values of the array $a$, you may output any of them.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 3 \cdot 10^5$)&nbsp;！ the size of the array and the number of modifications.</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$)&nbsp;！ the value of the array $c$ after the $q$ modifications.</p><p>The following $q$ lines each contain three integers $x_i$, $y_i$, and $z_i$ ($1 \leq x_i, y_i, z_i \leq n$)&nbsp;！ describing the $i$-th modification.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if $a$ exists, output $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$) in a single line. Otherwise, output "-1" in a single line.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 3 \cdot 10^5$)&nbsp;！ the size of the array and the number of modifications.</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$)&nbsp;！ the value of the array $c$ after the $q$ modifications.</p><p>The following $q$ lines each contain three integers $x_i$, $y_i$, and $z_i$ ($1 \leq x_i, y_i, z_i \leq n$)&nbsp;！ describing the $i$-th modification.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, if $a$ exists, output $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$) in a single line. Otherwise, output "-1" in a single line.</p><p>If there are multiple solutions, print any of them.</p>





```input1|2,3,4,9,10,11,12,13,14
3
2 1
1 2
2 1 2
3 2
1 2 3
2 3 2
1 2 1
6 4
1 2 2 3 4 5
5 6 6
4 5 5
3 4 4
2 3 3
```




```output1
-1
1 2 3 
1 2 3 4 5 5
```



## Note

<p>In the first test case, based on the given sequence of modifications, we know that $b_1 = a_1$ and $b_2 = \min(a_1, a_2)$. Therefore, it is necessary that $b_2 \leq b_1$. However, for the given $b$, we have $b_1&lt;b_2$. Therefore, there is no solution.</p><p>In the second test case, we can see that the given $c$ becomes $b$ from $a$ after the given modifications, and $c$ is not changed at each modification.</p>
