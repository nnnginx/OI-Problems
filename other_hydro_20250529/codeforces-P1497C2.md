## Description

<div><p><span class="tex-font-style-bf">It is the hard version of the problem. The only difference is that in this version $3 \le k \le n$.</span></p><p>You are given a positive integer $n$. Find $k$ positive integers $a_1, a_2, \ldots, a_k$, such that:</p><ul> <li> $a_1 + a_2 + \ldots + a_k = n$ </li><li> $LCM(a_1, a_2, \ldots, a_k) \le \frac{n}{2}$ </li></ul><p>Here $LCM$ is the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> of numbers $a_1, a_2, \ldots, a_k$.</p><p>We can show that for given constraints the answer always exists.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 10^4)$ &nbsp;�� the number of test cases.</p><p>The only line of each test case contains two integers $n$, $k$ ($3 \le n \le 10^9$, $3 \le k \le n$).</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print $k$ positive integers $a_1, a_2, \ldots, a_k$, for which all conditions are satisfied.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 10^4)$ &nbsp;�� the number of test cases.</p><p>The only line of each test case contains two integers $n$, $k$ ($3 \le n \le 10^9$, $3 \le k \le n$).</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print $k$ positive integers $a_1, a_2, \ldots, a_k$, for which all conditions are satisfied.</p>

## Samples

```input1
2
6 4
9 5
```

```output1
1 2 2 1 
1 3 3 1 1
```



