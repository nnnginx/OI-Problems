## Description

<div><p>You are given a tree with $n$ nodes numbered from $1$ to $n$, along with an array of size $n$. The value of $i$-th node is $a_{i}$. There are $q$ queries. In each query, you are given 2 nodes numbered as $x$ and $y$. </p><p>Consider the path from the node numbered as $x$ to the node numbered as $y$. Let the path be represented by $x = p_0, p_1, p_2, \ldots, p_r = y$, where $p_i$ are the intermediate nodes. Compute the sum of $a_{p_i}\oplus i$ for each $i$ such that $0 \le i \le r$ where $\oplus$ is the <a href="https://en.wikipedia.org/wiki/Exclusive_or">XOR</a> operator. </p><p>More formally, compute $$\sum_{i =0}^{r} a_{p_i}\oplus i$$. </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Each test case contains several sets of input data.</p><p>The first line of each set of input data contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;！ the number of nodes.</p><p>The next $n-1$ lines of each set of input data contain $2$ integers, $u$ and $v$ representing an edge between the node numbered $u$ and the node numbered $v$. It is guaranteed that $u \ne v$ and that the edges form a tree. </p><p>The next line of each set of input data contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 5 \cdot 10^5$)&nbsp;！ values of the nodes.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;！ the number of queries.</p><p>The next $q$ lines describe the queries. The $i$-th query contains $2$ integers $x$ and $y$ ($1 \le x,y \le n$) denoting the starting and the ending node of the path. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$ and sum of $q$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each query, output a single number&nbsp;！ the sum from the problem statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Each test case contains several sets of input data.</p><p>The first line of each set of input data contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;！ the number of nodes.</p><p>The next $n-1$ lines of each set of input data contain $2$ integers, $u$ and $v$ representing an edge between the node numbered $u$ and the node numbered $v$. It is guaranteed that $u \ne v$ and that the edges form a tree. </p><p>The next line of each set of input data contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 5 \cdot 10^5$)&nbsp;！ values of the nodes.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;！ the number of queries.</p><p>The next $q$ lines describe the queries. The $i$-th query contains $2$ integers $x$ and $y$ ($1 \le x,y \le n$) denoting the starting and the ending node of the path. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$ and sum of $q$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each query, output a single number&nbsp;！ the sum from the problem statement.</p>





```input1|2,3,4,5,6,7,8,9,10
1
4
1 2
2 3
3 4
2 3 6 5
3
1 4
3 4
1 1
```




```output1
14
10
2
```


