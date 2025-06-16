## Description

<div><p>Given integers $n$ and $k$, construct a sequence of $n$ non-negative (i.e. $\geq 0$) integers $a_1, a_2, \ldots, a_n$ such that </p><ol> <li> $\sum\limits_{i = 1}^n a_i = k$ </li><li> The <span class="tex-font-style-bf">number</span> of $1$s in the binary representation of $a_1 | a_2 | \ldots | a_n$ is maximized, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. </li></ol></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 10^9$)&nbsp;！ the number of non-negative integers to be printed and the sum respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a sequence $a_1, a_2, \ldots, a_n$ on a new line that satisfies the conditions given above.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 10^9$)&nbsp;！ the number of non-negative integers to be printed and the sum respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a sequence $a_1, a_2, \ldots, a_n$ on a new line that satisfies the conditions given above.</p><p>If there are multiple solutions, print any of them.</p>





```input1|2,4
4
1 5
2 3
2 5
6 51
```




```output1
5
1 2
5 0
3 1 1 32 2 12
```



## Note

<p>In the first test case, we have to print exactly one integer, hence we can only output $5$ as the answer.</p><p>In the second test case, we output $1, 2$ which sum up to $3$, and $1 | 2 = (11)_2$ has two $1$s in its binary representation, which is the maximum we can achieve in these constraints.</p><p>In the fourth test case, we output $3, 1, 1, 32, 2, 12$ which sum up to $51$, and $3 | 1 | 1 | 32 | 2 | 12 = (101\,111)_2$ has five $1$s in its binary representation, which is the maximum we can achieve in these constraints.</p>
