## Description

<div><p>Only a few know that Pan and Apollo weren't only battling for the title of the GOAT musician. A few millenniums later, they also challenged each other in math (or rather in fast calculations). The task they got to solve is the following:</p><p>Let $x_1, x_2, \ldots, x_n$ be the sequence of $n$ non-negative integers. Find this value: $$\sum_{i=1}^n \sum_{j=1}^n \sum_{k=1}^n (x_i \, \&amp; \, x_j) \cdot (x_j \, | \, x_k)$$</p><p>Here $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise and,</a> and $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise or.</a></p><p>Pan and Apollo could solve this in a few seconds. Can you do it too? For convenience, find the answer modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 1\,000$) denoting the number of test cases, then $t$ test cases follow.</p><p>The first line of each test case consists of a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$), the length of the sequence. The second one contains $n$ non-negative integers $x_1, x_2, \ldots, x_n$ ($0 \leq x_i &lt; 2^{60}$), elements of the sequence.</p><p>The sum of $n$ over all test cases will not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines. The $i$-th line should contain the answer to the $i$-th text case.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 1\,000$) denoting the number of test cases, then $t$ test cases follow.</p><p>The first line of each test case consists of a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$), the length of the sequence. The second one contains $n$ non-negative integers $x_1, x_2, \ldots, x_n$ ($0 \leq x_i &lt; 2^{60}$), elements of the sequence.</p><p>The sum of $n$ over all test cases will not exceed $5 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines. The $i$-th line should contain the answer to the $i$-th text case.</p>

## Samples

```input1
8
2
1 7
3
1 2 4
4
5 5 5 5
5
6 2 2 1 0
1
0
1
1
6
1 12 123 1234 12345 123456
5
536870912 536870911 1152921504606846975 1152921504606846974 1152921504606846973
```

```output1
128
91
1600
505
0
1
502811676
264880351
```



