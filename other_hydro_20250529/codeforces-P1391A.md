## Description

<div><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>For a positive integer $n$, we call a permutation $p$ of length $n$ <span class="tex-font-style-bf">good</span> if the following condition holds for every pair $i$ and $j$ ($1 \le i \le j \le n$)&nbsp;�� </p><ul> <li> $(p_i \text{ OR } p_{i+1} \text{ OR } \ldots \text{ OR } p_{j-1} \text{ OR } p_{j}) \ge j-i+1$, where $\text{OR}$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation.</a> </li></ul><p>In other words, a permutation $p$ is <span class="tex-font-style-bf">good</span> if for every subarray of $p$, the $\text{OR}$ of all elements in it is not less than the number of elements in that subarray. </p><p>Given a positive integer $n$, output any <span class="tex-font-style-bf">good</span> permutation of length $n$. We can show that for the given constraints such a permutation always exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first and only line of every test case contains a single integer $n$ ($1 \le n \le 100$).</p></div><div class="output-specification"><p>For every test, output any <span class="tex-font-style-bf">good</span> permutation of length $n$ on a separate line. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first and only line of every test case contains a single integer $n$ ($1 \le n \le 100$).</p>

## Output

<p>For every test, output any <span class="tex-font-style-bf">good</span> permutation of length $n$ on a separate line. </p>

## Samples

```input1
3
1
3
7
```

```output1
1
3 1 2
4 3 5 2 7 1 6
```




## Note

<p>For $n = 3$, $[3,1,2]$ is a good permutation. Some of the subarrays are listed below. </p><ul> <li> $3\text{ OR }1 = 3 \geq 2$ $(i = 1,j = 2)$ </li><li> $3\text{ OR }1\text{ OR }2 = 3 \geq 3$ $(i = 1,j = 3)$ </li><li> $1\text{ OR }2 = 3 \geq 2$ $(i = 2,j = 3)$ </li><li> $1 \geq 1$ $(i = 2,j = 2)$ </li></ul><p>Similarly, you can verify that $[4,3,5,2,7,1,6]$ is also good.</p>
