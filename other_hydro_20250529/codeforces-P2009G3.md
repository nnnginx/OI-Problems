## Description

<div><p><span class="tex-font-style-bf">This is the extreme version of the problem. In this version, the output of each query is different from the easy and hard versions. It is also guaranteed that $r \geq l+k-1$ for all queries.</span></p><p>For an arbitrary array $b$, Yunli can perform the following operation any number of times:</p><ul> <li> Select an index $i$. Set $b_i = x$ where $x$ is any integer she desires ($x$ is not limited to the interval $[1,n]$). </li></ul><p>Denote $f(b)$ as the minimum number of operations she needs to perform until there exists a consecutive subarray$^{\text{∗}}$ of length at least $k$ in $b$.</p><p>Yunli is given an array $a$ of size $n$ and asks you $q$ queries. In each query, you must output $\sum_{i=l}^{r-k+1} \sum_{j=i+k-1}^{r} f([a_i, a_{i+1}, \ldots, a_j])$.</p><div class="statement-footnote"><p>$^{\text{∗}}$If there exists a consecutive subarray of length $k$ that starts at index $i$ ($1 \leq i \leq |b|-k+1$), then $b_j = b_{j-1} + 1$ for all $i &lt; j \leq i+k-1$.</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r \geq l+k-1$) — the bounds of the query.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $\sum_{i=l}^{r-k+1} \sum_{j=i+k-1}^{r} f([a_i, a_{i+1}, \ldots, a_j])$ for each query on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r \geq l+k-1$) — the bounds of the query.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $\sum_{i=l}^{r-k+1} \sum_{j=i+k-1}^{r} f([a_i, a_{i+1}, \ldots, a_j])$ for each query on a new line.</p>





```input1|2,3,4,5,6,7,12,13,14,15,26,27,28,29,30,31
5
7 2 4
1 2 3 2 1 2 3
4 6
1 7
2 7
3 7
8 4 2
4 3 1 1 2 4 3 2
3 6
1 5
5 4 2
4 5 1 2 3
1 4
1 5
10 4 8
2 3 6 5 8 9 8 10 10 1
2 7
6 10
1 9
1 6
3 9
4 10
2 10
1 8
10 7 4
3 4 5 3 4 5 9 10 8 9
1 9
2 10
1 10
2 9
```




```output1
1
3
3
3
2
7
2
4
8
6
28
7
16
20
32
19
18
15
26
9
```



## Note

<p>In the first query of the first testcase, we can calculate the answer for the query through the following: </p><ul> <li> $i = 4$ and $j = 5$: $f([2, 1])=1$ because Yunli can set $b_2=3$, making a consecutive subarray of size $2$ in $1$ move. </li><li> $i = 4$ and $j = 6$: $f([2, 1, 2])=0$ because there is already a consecutive array of size $2$. </li><li> $i = 5$ and $j = 6$: $f([1, 2])=0$ because there is already a consecutive array of size $2$. </li></ul><p>The answer to this query is $1+0+0=1$.</p>
