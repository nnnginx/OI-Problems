## Description

<div><p>The beauty of an array $b$ of length $m$ is defined as $\max(b_i \oplus b_j)$ among all possible pairs $1 \le i \le j \le m$, where $x \oplus y$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of numbers $x$ and $y$. We denote the beauty value of the array $b$ as $f(b)$.</p><p>An array $b$ is called beautiful if $f(b) \ge k$.</p><p>Recently, Kostya bought an array $a$ of length $n$ from the store. He considers this array too long, so he plans to cut out some beautiful subarray from it. That is, he wants to choose numbers $l$ and $r$ ($1 \le l \le r \le n$) such that the array $a_{l \dots r}$ is beautiful. The length of such a subarray will be the number $r - l + 1$. The entire array $a$ is also considered a subarray (with $l = 1$ and $r = n$).</p><p>Your task is to find the length of the shortest beautiful subarray in the array $a$. If no subarray is beautiful, you should output the number $-1$.</p></div><div class="input-specification"><p>The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>Next, there are $t$ blocks of two lines:</p><p>In the first line of the block, there are two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$).</p><p>In the second line of the block, there is the array $a$ consisting of $n$ integers ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ across all tests does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, you need to output a single integer ¡ª the minimum length of the segment $(l, r)$ for which $f(a_{l \dots r}) \ge k$. If such a segment is not found, you should output $-1$.</p></div>

## Input

<p>The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>Next, there are $t$ blocks of two lines:</p><p>In the first line of the block, there are two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$).</p><p>In the second line of the block, there is the array $a$ consisting of $n$ integers ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ across all tests does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, you need to output a single integer ¡ª the minimum length of the segment $(l, r)$ for which $f(a_{l \dots r}) \ge k$. If such a segment is not found, you should output $-1$.</p>





```input1|2,3,6,7,10,11
6
5 0
1 2 3 4 5
5 7
1 2 3 4 5
5 8
1 2 3 4 5
5 7
3 5 1 4 2
5 3
3 5 1 4 2
6 71
26 56 12 45 60 27
```




```output1
1
2
-1
4
2
-1
```


