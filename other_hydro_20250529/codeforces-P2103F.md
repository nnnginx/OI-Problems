## Description

<div><p>  </p><p>The bitwise nor$^{\text{∗}}$ of an array of $k$-bit integers $b_1, b_2, \ldots, b_m$ can be computed by calculating the bitwise nor cumulatively from left to right. More formally, $\operatorname{nor}(b_1, b_2, \ldots, b_m) = \operatorname{nor}(\operatorname{nor}(b_1, b_2, \ldots, b_{m - 1}), b_m)$ for $m\ge 2$, and $\operatorname{nor}(b_1) = b_1$.</p><p>You are given an array of $k$-bit integers $a_1, a_2, \ldots, a_n$. For each index $i$ ($1\le i\le n$), find the maximum bitwise nor among all subarrays$^{\text{†}}$ of $a$ containing index $i$. In other words, for each index $i$, find the maximum value of $\operatorname{nor}(a_l, a_{l+1}, \ldots, a_r)$ among all $1 \le l \le i \le r \le n$.</p><div class="statement-footnote"><p>$^{\text{∗}}$ The <a href="https://en.m.wikipedia.org/wiki/Logical_NOR">logical nor</a> of two boolean values is $1$ if both values are $0$, and $0$ otherwise. The bitwise nor of two $k$-bit integers is calculated by performing the logical nor operation on each pair of the corresponding bits.</p><p>For example, let us compute $\operatorname{nor}(2, 6)$ when they are represented as $4$-bit numbers. In binary, $2$=$0010_2$ and $6=0110_2$. Therefore, $\operatorname{nor}(2,6) = 1001_2 = 9$ as by performing the logical nor operations from left to right, we have:</p><ul> <li> $\operatorname{nor}(0,0) = 1$ </li><li> $\operatorname{nor}(0,1) = 0$ </li><li> $\operatorname{nor}(1,0) = 0$ </li><li> $\operatorname{nor}(1,1) = 0$ </li></ul><p>Note that if $2$ and $6$ were represented as $3$-bit integers instead, then $\operatorname{nor}(2,6) = 1$. </p><p>$^{\text{†}}$An array $x$ is a subarray of an array $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $1 \le k \le 17$)&nbsp;— the number of elements in the array and the number of bits of the array elements.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 2^k - 1$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p></div><div class="output-specification"><p>For each test case, output $n$ integers, the $i$-th of which is the maximum bitwise nor among all subarrays of $a$ containing index $i$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $1 \le k \le 17$)&nbsp;— the number of elements in the array and the number of bits of the array elements.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 2^k - 1$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p>

## Output

<p>For each test case, output $n$ integers, the $i$-th of which is the maximum bitwise nor among all subarrays of $a$ containing index $i$.</p>





```input1|2,3
2
2 2
1 3
5 3
1 7 4 6 2
```




```output1
1 3
5 7 5 6 5
```



## Note

<p>In the first test case, subarrays that have index $1$ are $[1]$ and $[1, 3]$. The values of their bitwise nor are $1$ and $0$ respectively. Hence, the answer for index $1$ is $1$. Subarrays that have index $2$ are $[3]$ and $[1, 3]$. The values of their bitwise nor are $3$ and $0$ respectively. Hence, the answer for index $2$ is $3$.</p><p>In the second test case: </p><ul> <li> For $i = 1$, the subarray with maximum bitwise nor is $[a_1, a_2, a_3, a_4, a_5] = [1, 7, 4, 6, 2]$, $\operatorname{nor}(1, 7, 4, 6, 2) = 5$ </li><li> For $i = 2$, the subarray with maximum bitwise nor is $[a_2] = [7]$, $\operatorname{nor}(7) = 7$ </li><li> For $i = 3$, the subarray with maximum bitwise nor is $[a_1, a_2, a_3, a_4, a_5] = [1, 7, 4, 6, 2]$, $\operatorname{nor}(1, 7, 4, 6, 2) = 5$ </li><li> For $i = 4$, the subarray with maximum bitwise nor is $[a_4] = [6]$, $\operatorname{nor}(6) = 6$ </li><li> For $i = 5$, the subarray with maximum bitwise nor is $[a_1, a_2, a_3, a_4, a_5] = [1, 7, 4, 6, 2]$, $\operatorname{nor}(1, 7, 4, 6, 2) = 5$ </li></ul>
