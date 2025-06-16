## Description

<div><p>You have an array of non-negative integers $a_1, a_2, \ldots, a_n$.</p><p>The value of a sub-array of length $\ge 2$, $a[l, r] = [a_l, a_{l+1}, \ldots, a_r]$ is the minimum value of $a_i \oplus a_j$ such that $l \le i &lt; j \le r$, where $\oplus$ is the xor (exclusive-or) operator.</p><p>You have to find the $k$-th smallest value over all sub-arrays of length $\ge 2$.</p></div><div class="input-specification"><p>The first line of the input contains multiple test cases $t$ ($1 \le t \le 2 \cdot 10^4$).</p><p>The first line of each test case contains integer numbers $n$ and $k$ ($2 \le n \le 10^5$, $1 \le k \le \frac{n\cdot(n-1)}{2}$).</p><p>The second line of the input contains $n$ non-negative integer numbers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) ¡ª the array itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>Print the $k$-th smallest value obtained over all subarrays of length at least $2$.</p></div>

## Input

<p>The first line of the input contains multiple test cases $t$ ($1 \le t \le 2 \cdot 10^4$).</p><p>The first line of each test case contains integer numbers $n$ and $k$ ($2 \le n \le 10^5$, $1 \le k \le \frac{n\cdot(n-1)}{2}$).</p><p>The second line of the input contains $n$ non-negative integer numbers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) ¡ª the array itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>Print the $k$-th smallest value obtained over all subarrays of length at least $2$.</p>





```input1|2,3,6,7
4
5 2
1 2 3 4 5
2 1
4 3
4 6
1 2 4 8
5 9
1 2 3 4 5
```




```output1
1
7
12
3
```



## Note

<p>In the first testcase, we have subarrays with their smallest exclusive-or pair as:</p><p>$[1,2]: 3$</p><p>$[2,3]: 1$</p><p>$[3,4]: 7$</p><p>$[4,5]: 1$</p><p>$[1,2,3]: 1$</p><p>$[2,3,4]: 1$</p><p>$[3,4,5]: 1$</p><p>$[1,2,3,4]: 1$</p><p>$[2,3,4,5]: 1$</p><p>$[1,2,3,4,5]: 1$</p><p>The sorted order would be: $1, 1, 1, 1, 1, 1, 1, 1, 3, 7$. Therefore, the second smallest element would be $1$. </p>
