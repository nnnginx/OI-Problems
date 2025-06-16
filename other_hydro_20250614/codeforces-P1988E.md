## Description

<div><p>For an array $[a_1,a_2,\ldots,a_n]$ of length $n$, define $f(a)$ as the sum of the minimum element over all subsegments. That is, $$f(a)=\sum_{l=1}^n\sum_{r=l}^n \min_{l\le i\le r}a_i.$$</p><p>A permutation is a sequence of integers from $1$ to $n$ of length $n$ containing each number exactly once. You are given a permutation $[a_1,a_2,\ldots,a_n]$. For each $i$, solve the following problem independently:</p><ul> <li> Erase $a_i$ from $a$, concatenating the remaining parts, resulting in $b = [a_1,a_2,\ldots,a_{i-1},\;a_{i+1},\ldots,a_{n}]$. </li><li> Calculate $f(b)$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1\le n\le 5\cdot 10^5$).</p><p>The second line of each test case contains $n$ distinct integers $a_1,\ldots,a_n$ ($1\le a_i\le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print one line containing $n$ integers. The $i$-th integer should be the answer when erasing $a_i$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1\le n\le 5\cdot 10^5$).</p><p>The second line of each test case contains $n$ distinct integers $a_1,\ldots,a_n$ ($1\le a_i\le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print one line containing $n$ integers. The $i$-th integer should be the answer when erasing $a_i$.</p>





```input1|2,3,6,7
4
1
1
3
3 1 2
5
4 2 1 5 3
8
8 1 4 6 7 3 5 2
```




```output1
0 
4 7 5 
19 21 27 17 19 
79 100 72 68 67 80 73 80
```



## Note

<p>In the second test case, $a=[3,1,2]$.</p><ul> <li> When removing $a_1$, $b=[1,2]$. $f(b)=1+2+\min\{1,2\}=4$. </li><li> When removing $a_2$, $b=[3,2]$. $f(b)=3+2+\min\{3,2\}=7$. </li><li> When removing $a_3$, $b=[3,1]$. $f(b)=3+1+\min\{3,1\}=5$. </li></ul>
