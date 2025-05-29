## Description

<div><p>For a certain permutation $p$$^{\text{∗}}$ Sakurako calls an integer $j$ reachable from an integer $i$ if it is possible to make $i$ equal to $j$ by assigning $i=p_i$ a certain number of times.</p><p>If $p=[3,5,6,1,2,4]$, then, for example, $4$ is reachable from $1$, because: $i=1$ $\rightarrow$ $i=p_1=3$ $\rightarrow$ $i=p_3=6$ $\rightarrow$ $i=p_6=4$. Now $i=4$, so $4$ is reachable from $1$.</p><p>Each number in the permutation is colored either black or white.</p><p>Sakurako defines the function $F(i)$ as the number of black integers that are reachable from $i$.</p><p>Sakurako is interested in $F(i)$ for each $1\le i\le n$, but calculating all values becomes very difficult, so she asks you, as her good friend, to compute this.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation (the number $2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$, but the array contains $4$).</p></div></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) &nbsp;— the number of elements in the array.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \dots, p_n$ ($1\le p_i\le n$) &nbsp;— the elements of the permutation.</p><p>The third line of each test case contains a string $s$ of length $n$, consisting of '0' and '1'. If $s_i=0$, then the number $p_i$ is colored black; if $s_i=1$, then the number $p_i$ is colored white.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $F(1), F(2), \dots, F(n)$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) &nbsp;— the number of elements in the array.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \dots, p_n$ ($1\le p_i\le n$) &nbsp;— the elements of the permutation.</p><p>The third line of each test case contains a string $s$ of length $n$, consisting of '0' and '1'. If $s_i=0$, then the number $p_i$ is colored black; if $s_i=1$, then the number $p_i$ is colored white.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers $F(1), F(2), \dots, F(n)$.</p>





```input1|2,3,4,8,9,10,14,15,16
5
1
1
0
5
1 2 4 5 3
10101
5
5 4 1 3 2
10011
6
3 5 6 1 2 4
010000
6
1 2 3 4 5 6
100110
```




```output1
1 
0 1 1 1 1 
2 2 2 2 2 
4 1 4 4 1 4 
0 1 1 0 0 1
```


