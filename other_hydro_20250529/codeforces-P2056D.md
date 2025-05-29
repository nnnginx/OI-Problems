## Description

<div><p>  </p><p>An array $b$ of $m$ integers is called <span class="tex-font-style-it">good</span> if, <span class="tex-font-style-bf">when it is sorted</span>, $b_{\left\lfloor \frac{m + 1}{2} \right\rfloor} = b_{\left\lceil \frac{m + 1}{2} \right\rceil}$. In other words, $b$ is good if both of its medians are equal. In particular, $\left\lfloor \frac{m + 1}{2} \right\rfloor = \left\lceil \frac{m + 1}{2} \right\rceil$ when $m$ is odd, so $b$ is guaranteed to be good if it has an odd length.</p><p>You are given an array $a$ of $n$ integers. Calculate the number of good subarrays$^{\text{∗}}$ in $a$.</p><div class="statement-footnote"><p>$^{\text{∗}}$An array $x$ is a subarray of an array $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le \color{red}{\textbf{10}}$)&nbsp;— the given array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer representing the number of good subarrays in $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le \color{red}{\textbf{10}}$)&nbsp;— the given array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p>

## Output

<p>For each test case, output a single integer representing the number of good subarrays in $a$.</p>





```input1|2,3,6,7
3
4
1 1 1 1
5
1 10 2 3 3
10
6 3 2 3 5 3 4 2 3 5
```




```output1
10
11
42
```



## Note

<p>In the first case, every subarray is good since all its elements are equal to $1$.</p><p>In the second case, an example of a good subarray is $b = [10, 2, 3, 3]$. When it is sorted, $b = [2, 3, 3, 10]$, so $b_{\left\lfloor \frac{4 + 1}{2} \right\rfloor} = b_{\left\lceil \frac{4 + 1}{2} \right\rceil} = b_2 = b_3 = 3$. Another example would be $b = [1, 10, 2]$. On the other hand, $b = [1, 10]$ is not good as its two medians are $1$ and $10$, which are not equal.</p>
