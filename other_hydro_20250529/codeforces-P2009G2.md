## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. In this version, it is guaranteed that $r \geq l+k-1$ for all queries.</span></p><p>For an arbitrary array $b$, Yunli can perform the following operation any number of times:</p><ul> <li> Select an index $i$. Set $b_i = x$ where $x$ is any integer she desires ($x$ is not limited to the interval $[1,n]$). </li></ul><p>Denote $f(b)$ as the minimum number of operations she needs to perform until there exists a consecutive subarray$^{\text{∗}}$ of length at least $k$ in $b$.</p><p>Yunli is given an array $a$ of size $n$ and asks you $q$ queries. In each query, you must output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$.</p><div class="statement-footnote"><p>$^{\text{∗}}$If there exists a consecutive subarray of length $k$ that starts at index $i$ ($1 \leq i \leq |b|-k+1$), then $b_j = b_{j-1} + 1$ for all $i &lt; j \leq i+k-1$.</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r \geq l+k-1$) — the bounds of the query.</p><p>It is guaranteed the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$ for each query on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, ..., a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r \geq l+k-1$) — the bounds of the query.</p><p>It is guaranteed the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$ for each query on a new line.</p>





```input1|2,3,4,5,6,11,12,13,14
3
7 5 3
1 2 3 2 1 2 3
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
```




```output1
6
5
2
2
5
2
3
```



## Note

<p>In the second query of the first testcase, we calculate the following function values: </p><ul> <li> $f([2,3,2,1,2])=3$ because Yunli can set $b_3=4$, $b_4=5$, and $b_5=6$, making a consecutive subarray of size $5$ in $3$ moves. </li><li> $f([2,3,2,1,2,3]=2$ because we can set $b_3=0$ and $b_2=-1$, making a consecutive subarray of size $5$ in $2$ moves (starting at position $2$) </li></ul><p>The answer to this query is $3+2=5$.</p>
