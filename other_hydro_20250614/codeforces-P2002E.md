## Description

<div><p>Given an array of integers $s_1, s_2, \ldots, s_l$, every second, cosmic rays will cause all $s_i$ such that $i=1$ or $s_i\neq s_{i-1}$ to be deleted simultaneously, and the remaining parts will be concatenated together in order to form the new array $s_1, s_2, \ldots, s_{l'}$.</p><p>Define the <span class="tex-font-style-bf">strength</span> of an array as the number of seconds it takes to become empty.</p><p>You are given an array of integers compressed in the form of $n$ pairs that describe the array left to right. Each pair $(a_i,b_i)$ represents $a_i$ copies of $b_i$, i.e. $\underbrace{b_i,b_i,\cdots,b_i}_{a_i\textrm{ times}}$.</p><p>For each $i=1,2,\dots,n$, please find the <span class="tex-font-style-bf">strength</span> of the sequence described by the first $i$ pairs.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le3\cdot10^5$)&nbsp;！ the length of sequence $a$.</p><p>The next $n$ lines contain two integers each $a_i$, $b_i$ ($1\le a_i\le10^9,0\le b_i\le n$)&nbsp;！ the pairs which describe the sequence. </p><p>It is guaranteed that the sum of all $n$ does not exceed $3\cdot10^5$.</p><p>It is guaranteed that for all $1\le i&lt;n$, $b_i\neq b_{i+1}$ holds.</p></div><div class="output-specification"><p>For each test case, print one line containing $n$ integers&nbsp;！ the answer for each prefix of pairs.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le3\cdot10^5$)&nbsp;！ the length of sequence $a$.</p><p>The next $n$ lines contain two integers each $a_i$, $b_i$ ($1\le a_i\le10^9,0\le b_i\le n$)&nbsp;！ the pairs which describe the sequence. </p><p>It is guaranteed that the sum of all $n$ does not exceed $3\cdot10^5$.</p><p>It is guaranteed that for all $1\le i&lt;n$, $b_i\neq b_{i+1}$ holds.</p>

## Output

<p>For each test case, print one line containing $n$ integers&nbsp;！ the answer for each prefix of pairs.</p>





```input1|2,3,4,5,6,14,15,16,17,18,19,20,21
4
4
2 0
1 1
3 0
5 1
6
4 6
1 3
4 6
4 0
7 6
6 3
7
9 0
7 1
5 0
7 1
9 0
1 1
2 0
10
10 7
4 9
2 2
7 9
2 8
8 5
11 7
15 5
12 7
4 0
```




```output1
2 2 4 5 
4 4 7 7 10 10 
9 9 9 9 9 9 10 
10 10 10 10 10 10 12 15 15 15
```



## Note

<p>In the first test case, for the prefix of length $4$, the changes will be $[0,0,1,0,0,0,1,1,1,1,1]\rightarrow[0,0,0,1,1,1,1]\rightarrow[0,0,1,1,1]\rightarrow[0,1,1]\rightarrow[1]\rightarrow[]$, so the array becomes empty after $5$ seconds.</p><p>In the second test case, for the prefix of length $4$, the changes will be $[6,6,6,6,3,6,6,6,6,0,0,0,0]\rightarrow[6,6,6,6,6,6,0,0,0]\rightarrow[6,6,6,6,6,0,0]\rightarrow[6,6,6,6,0]\rightarrow[6,6,6]\rightarrow[6,6]\rightarrow[6]\rightarrow[]$, so the array becomes empty after $7$ seconds.</p>
