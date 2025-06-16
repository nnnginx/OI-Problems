## Description

<div><p>Polycarp was given an array $a$ of $n$ integers. He really likes triples of numbers, so for each $j$ ($1 \le j \le n - 2$) he wrote down a triple of elements $[a_j, a_{j + 1}, a_{j + 2}]$.</p><p>Polycarp considers a pair of triples $b$ and $c$ <span class="tex-font-style-it">beautiful</span> if they differ in exactly one position, that is, one of the following conditions is satisfied:</p><ul> <li> $b_1 \ne c_1$ and $b_2 = c_2$ and $b_3 = c_3$; </li><li> $b_1 = c_1$ and $b_2 \ne c_2$ and $b_3 = c_3$; </li><li> $b_1 = c_1$ and $b_2 = c_2$ and $b_3 \ne c_3$. </li></ul><p>Find the number of <span class="tex-font-style-it">beautiful</span> pairs of triples among the written triples $[a_j, a_{j + 1}, a_{j + 2}]$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of the values of $n$ for all test cases in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of <span class="tex-font-style-it">beautiful</span> pairs of triples among the pairs of the form $[a_j, a_{j + 1}, a_{j + 2}]$.</p><p>Note that the answer may not fit into 32-bit data types.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of the values of $n$ for all test cases in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of <span class="tex-font-style-it">beautiful</span> pairs of triples among the pairs of the form $[a_j, a_{j + 1}, a_{j + 2}]$.</p><p>Note that the answer may not fit into 32-bit data types.</p>





```input1|2,3,6,7,10,11,14,15
8
5
3 2 2 2 3
5
1 2 1 2 1
8
1 2 3 2 2 3 4 2
4
2 1 1 1
8
2 1 1 2 1 1 1 1
7
2 1 1 1 1 1 1
6
2 1 1 1 1 1
5
2 1 1 1 1
```




```output1
2
0
3
1
8
4
3
2
```



## Note

<p>In the first example, $a = [3, 2, 2, 2, 3]$, Polycarp will write the following triples: </p><ol> <li> $[3, 2, 2]$; </li><li> $[2, 2, 2]$; </li><li> $[2, 2, 3]$. </li></ol> The beautiful pairs are triple $1$ with triple $2$ and triple $2$ with triple $3$.<p>In the third example, $a = [1, 2, 3, 2, 2, 3, 4, 2]$, Polycarp will write the following triples: </p><ol> <li> $[1, 2, 3]$; </li><li> $[2, 3, 2]$; </li><li> $[3, 2, 2]$; </li><li> $[2, 2, 3]$; </li><li> $[2, 3, 4]$; </li><li> $[3, 4, 2]$; </li></ol> The beautiful pairs are triple $1$ with triple $4$, triple $2$ with triple $5$, and triple $3$ with triple $6$.
