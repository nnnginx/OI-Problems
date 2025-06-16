## Description

<div><p>   </p><p>You are given a permutation $a$ of length $n$$^{\text{∗}}$. You are allowed to do the following operation any number of times (possibly zero):</p><ul> <li> Choose an index $1\le i\le n - 3$. Then, swap $a_i$ with $a_{i + 2}$, and $a_{i + 1}$ with $a_{i + 3}$ simultaneously. In other words, permutation $a$ will be transformed from $[\ldots, a_i, a_{i+1}, a_{i+2}, a_{i+3}, \ldots]$ to $[\ldots, a_{i+2}, a_{i+3}, a_{i}, a_{i+1}, \ldots]$. </li></ul><p>Determine the lexicographically smallest permutation$^{\text{†}}$ that can be obtained by applying the above operation any number of times.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). </p><p>$^{\text{†}}$An array $x$ is lexicographically smaller than an array $y$ of the same size if and only if the following holds: </p><ul> <li> in the first position where $x$ and $y$ differ, the array $x$ has a smaller element than the corresponding element in $y$. </li></ul> </div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($4\le n\le 2\cdot 10^5$)&nbsp;— the length of permutation $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of permutation $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output the lexicographically smallest permutation that can be obtained by applying the above operation any number of times.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($4\le n\le 2\cdot 10^5$)&nbsp;— the length of permutation $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of permutation $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$. </p>

## Output

<p>For each test case, output the lexicographically smallest permutation that can be obtained by applying the above operation any number of times.</p>





```input1|2,3,6,7
3
4
3 4 1 2
5
5 4 3 1 2
10
10 9 8 7 6 5 4 3 2 1
```




```output1
1 2 3 4 
2 1 3 4 5 
2 1 4 3 6 5 8 7 10 9
```



## Note

<p>In the first test case, an operation can be done on index $i = 1$, and the permutation will become $[1, 2, 3, 4]$, which is the lexicographically smallest permutation achievable.</p><p>In the second test case, we can do the following sequence of operations:</p><ul> <li> Do an operation on index $i = 2$. The permutation becomes $[5, 1, 2, 4, 3]$. </li><li> Do an operation on index $i = 1$. The permutation becomes $[2, 4, 5, 1, 3]$. </li><li> Do an operation on index $i = 2$. The permutation becomes $[2, 1, 3, 4, 5]$. </li></ul>
