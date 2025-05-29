## Description

<div><p>Initially, we had one array, which was a permutation of size $n$ (an array of size $n$ where each integer from $1$ to $n$ appears exactly once).</p><p>We performed $q$ operations. During the $i$-th operation, we did the following:</p><ul> <li> choose any array we have with at least $2$ elements; </li><li> split it into two non-empty arrays (prefix and suffix); </li><li> write two integers $l_i$ and $r_i$, where $l_i$ is the maximum element in the left part which we get after the split, and $r_i$ is the maximum element in the right part; </li><li> remove the array we've chosen from the pool of arrays we can use, and add the two resulting parts into the pool. </li></ul><p>For example, suppose the initial array was $[6, 3, 4, 1, 2, 5]$, and we performed the following operations:</p><ol> <li> choose the array $[6, 3, 4, 1, 2, 5]$ and split it into $[6, 3]$ and $[4, 1, 2, 5]$. Then we write $l_1 = 6$ and $r_1 = 5$, and the arrays we have are $[6, 3]$ and $[4, 1, 2, 5]$; </li><li> choose the array $[4, 1, 2, 5]$ and split it into $[4, 1, 2]$ and $[5]$. Then we write $l_2 = 4$ and $r_2 = 5$, and the arrays we have are $[6, 3]$, $[4, 1, 2]$ and $[5]$; </li><li> choose the array $[4, 1, 2]$ and split it into $[4]$ and $[1, 2]$. Then we write $l_3 = 4$ and $r_3 = 2$, and the arrays we have are $[6, 3]$, $[4]$, $[1, 2]$ and $[5]$. </li></ol><p>You are given two integers $n$ and $q$, and two sequences $[l_1, l_2, \dots, l_q]$ and $[r_1, r_2, \dots, r_q]$. A permutation of size $n$ is called <span class="tex-font-style-it">valid</span> if we can perform $q$ operations and produce the given sequences $[l_1, l_2, \dots, l_q]$ and $[r_1, r_2, \dots, r_q]$.</p><p>Calculate the number of valid permutations.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le q &lt; n \le 3 \cdot 10^5$).</p><p>The second line contains $q$ integers $l_1, l_2, \dots, l_q$ ($1 \le l_i \le n$).</p><p>The third line contains $q$ integers $r_1, r_2, \dots, r_q$ ($1 \le r_i \le n$).</p><p>Additional constraint on the input: there exists at least one permutation which can produce the given sequences $[l_1, l_2, \dots, l_q]$ and $[r_1, r_2, \dots, r_q]$.</p></div><div class="output-specification"><p>Print one integer ¡ª the number of valid permutations, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le q &lt; n \le 3 \cdot 10^5$).</p><p>The second line contains $q$ integers $l_1, l_2, \dots, l_q$ ($1 \le l_i \le n$).</p><p>The third line contains $q$ integers $r_1, r_2, \dots, r_q$ ($1 \le r_i \le n$).</p><p>Additional constraint on the input: there exists at least one permutation which can produce the given sequences $[l_1, l_2, \dots, l_q]$ and $[r_1, r_2, \dots, r_q]$.</p>

## Output

<p>Print one integer ¡ª the number of valid permutations, taken modulo $998244353$.</p>





```input1|
6 3
6 4 4
5 5 2
```




```input2|
10 1
10
9
```




```input3|
4 1
2
4
```




```output1
30
```




```output2
1814400
```




```output3
8
```


