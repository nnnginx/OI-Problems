## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. In this version, it is guaranteed that $r=l+k-1$ for all queries.</span></p><p>For an arbitrary array $b$, Yunli can perform the following operation any number of times:</p><ul> <li> Select an index $i$. Set $b_i = x$ where $x$ is any integer she desires ($x$ is not limited to the interval $[1,n]$). </li></ul><p>Denote $f(b)$ as the minimum number of operations she needs to perform until there exists a consecutive subarray$^{\text{∗}}$ of length at least $k$ in $b$.</p><p>Yunli is given an array $a$ of size $n$ and asks you $q$ queries. In each query, you must output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$. Note that in this version, you are only required to output $f([a_l, a_{l+1}, \ldots, a_{l+k-1}])$.</p><div class="statement-footnote"><p>$^{\text{∗}}$If there exists a consecutive subarray of length $k$ that starts at index $i$ ($1 \leq i \leq |b|-k+1$), then $b_j = b_{j-1} + 1$ for all $i &lt; j \leq i+k-1$.</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r=l+k-1$) — the bounds of the query.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$ for each query on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$ ($1 \leq k \leq n \leq 2 \cdot 10^5$, $1 \leq q \leq 2 \cdot 10^5$) — the length of the array, the length of the consecutive subarray, and the number of queries.</p><p>The following line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$).</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$, $r=l+k-1$) — the bounds of the query.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $\sum_{j=l+k-1}^{r} f([a_l, a_{l+1}, \ldots, a_j])$ for each query on a new line.</p>





```input1|2,3,4,5,6,11,12,13,14
3
7 5 3
1 2 3 2 1 2 3
1 5
2 6
3 7
8 4 2
4 3 1 1 2 4 3 2
3 6
2 5
5 4 2
4 5 1 2 3
1 4
2 5
```




```output1
2
3
2
2
2
2
1
```



## Note

<p>In the first query of the first testcase, $b=[1,2,3,2,1]$. Yunli can make a consecutive subarray of length $5$ in $2$ moves: </p><ul> <li> Set $b_4=4$ </li><li> Set $b_5=5$ </li></ul> After operations $b=[1, 2, 3, 4, 5]$.<p>In the second query of the first testcase, $b=[2,3,2,1,2]$. Yunli can make a consecutive subarray of length $5$ in $3$ moves: </p><ul> <li> Set $b_3=0$ </li><li> Set $b_2=-1$ </li><li> Set $b_1=-2$ </li></ul> After operations $b=[-2, -1, 0, 1, 2]$.
