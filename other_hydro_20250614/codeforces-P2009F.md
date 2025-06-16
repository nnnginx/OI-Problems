## Description

<div><p>Firefly is given an array $a$ of length $n$. Let $c_i$ denote the $i$'th cyclic shift$^{\text{∗}}$ of $a$. She creates a new array $b$ such that $b = c_1 + c_2 + \dots + c_n$ where $+$ represents concatenation$^{\text{†}}$. </p><p>Then, she asks you $q$ queries. For each query, output the sum of all elements in the subarray of $b$ that starts from the $l$-th element and ends at the $r$-th element, inclusive of both ends.</p><div class="statement-footnote"><p>$^{\text{∗}}$The $x$-th ($1 \leq x \leq n$) cyclic shift of the array $a$ is $a_x, a_{x+1} \ldots a_n, a_1, a_2 \ldots a_{x - 1}$. Note that the $1$-st shift is the initial $a$.</p><p>$^{\text{†}}$The concatenation of two arrays $p$ and $q$ of length $n$ (in other words, $p + q$) is $p_1, p_2, ..., p_n, q_1, q_2, ..., q_n$.</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$) — the length of the array and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq 10^6$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n^2$) — the left and right bounds of the query.</p><p><span class="tex-font-style-bf">Note that the large inputs may require the use of 64-bit integers.</span></p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each query, output the answer on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$) — the length of the array and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq 10^6$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n^2$) — the left and right bounds of the query.</p><p><span class="tex-font-style-bf">Note that the large inputs may require the use of 64-bit integers.</span></p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each query, output the answer on a new line.</p>





```input1|2,3,4,5,6,14,15,16,26,27,28,29,30
5
3 3
1 2 3
1 9
3 5
8 8
5 5
4 8 3 2 4
1 14
3 7
7 10
2 11
1 25
1 1
6
1 1
5 7
3 1 6 10 4
3 21
6 17
2 2
1 5
1 14
9 15
12 13
5 3
4 9 10 10 1
20 25
3 11
20 22
```




```output1
18
8
1
55
20
13
41
105
6
96
62
1
24
71
31
14
44
65
15
```



## Note

<p>For the first test case, $b = [1, 2, 3, 2, 3, 1, 3, 1, 2]$.</p>
