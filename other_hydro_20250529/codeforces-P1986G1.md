## Description

<div><p><span class="tex-font-style-bf">This is a simple version of the problem. The only difference is that in this version $n \leq 10^5$ and the sum of $n$ for all sets of input data does not exceed $10^5$.</span></p><p>You are given a permutation $p$ of length $n$. Calculate the number of index pairs $1 \leq i &lt; j \leq n$ such that $p_i \cdot p_j$ is divisible by $i \cdot j$ without remainder.</p><p>A permutation is a sequence of $n$ integers, where each integer from $1$ to $n$ occurs exactly once. For example, $[1]$, $[3,5,2,1,4]$, $[1,3,2]$ are permutations, while $[2,3,2]$, $[4,3,1]$, $[0]$ are not.</p></div><div class="input-specification"><p>Each test consists of multiple sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. Then follows their description.</p><p>The first line of each set of input data contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the length of the permutation $p$.</p><p>The second line of each set of input data contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;！ the permutation $p$.</p><p>It is guaranteed that the sum of $n$ for all sets of input data does not exceed $10^5$.</p></div><div class="output-specification"><p>For each set of input data, output the number of index pairs $1 \leq i &lt; j \leq n$ such that $p_i \cdot p_j$ is divisible by $i \cdot j$ without remainder.</p></div>

## Input

<p>Each test consists of multiple sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. Then follows their description.</p><p>The first line of each set of input data contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the length of the permutation $p$.</p><p>The second line of each set of input data contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;！ the permutation $p$.</p><p>It is guaranteed that the sum of $n$ for all sets of input data does not exceed $10^5$.</p>

## Output

<p>For each set of input data, output the number of index pairs $1 \leq i &lt; j \leq n$ such that $p_i \cdot p_j$ is divisible by $i \cdot j$ without remainder.</p>





```input1|2,3,6,7,10,11
6
1
1
2
1 2
3
2 3 1
5
2 4 1 3 5
12
8 9 7 12 1 10 6 3 2 4 11 5
15
1 2 4 6 8 10 12 14 3 9 15 5 7 11 13
```




```output1
0
1
1
3
9
3
```



## Note

<p>In the first set of input data, there are no index pairs, as the size of the permutation is $1$.</p><p>In the second set of input data, there is one index pair $(1, 2)$ and it is valid.</p><p>In the third set of input data, the index pair $(1, 2)$ is valid.</p><p>In the fourth set of input data, the index pairs $(1, 2)$, $(1, 5)$, and $(2, 5)$ are valid.</p>
