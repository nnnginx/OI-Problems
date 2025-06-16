## Description

<div><p>You are given an array $a$ consisting of $n$ nonnegative integers. </p><p>You can swap the elements at positions $i$ and $j$ if $a_i~\mathsf{XOR}~a_j &lt; 4$, where $\mathsf{XOR}$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Find the lexicographically smallest array that can be made with any number of swaps.</p><p>An array $x$ is lexicographically smaller than an array $y$ if in the first position where $x$ and $y$ differ, $x_i &lt; y_i$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 10^9$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers&nbsp;！ the lexicographically smallest array that can be made with any number of swaps.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 10^9$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers&nbsp;！ the lexicographically smallest array that can be made with any number of swaps.</p>





```input1|2,3,6,7
4
4
1 0 3 2
5
2 7 1 5 6
8
1 2 1 2 1 2 1 2
4
16 4 1 64
```




```output1
0 1 2 3 
1 5 2 6 7 
1 1 1 1 2 2 2 2 
16 4 1 64
```



## Note

<p>For the first test case, you can swap any two elements, so we can produce the sorted array.</p><p>For the second test case, you can swap $2$ and $1$ (their $\mathsf{XOR}$ is $3$), $7$ and $5$ (their $\mathsf{XOR}$ is $2$), and $7$ and $6$ (their $\mathsf{XOR}$ is $1$) to get the lexicographically smallest array.</p>
