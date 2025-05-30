## Description

<div><p>You are given a permutation $p$ of integers from $1$ to $n$, where $n$ is an even number. </p><p>Your goal is to sort the permutation. To do so, you can perform zero or more operations of the following type: </p><ul> <li> take two indices $i$ and $j$ such that $2 \cdot |i - j| \geq n$ and swap $p_i$ and $p_j$. </li></ul><p>There is <span class="tex-font-style-bf">no need to minimize</span> the number of operations, however you should use no more than $5 \cdot n$ operations. One can show that it is always possible to do that.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$, $n$ is even)&nbsp;！ the length of the permutation. </p><p>The second line contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;！ the given permutation.</p></div><div class="output-specification"><p>On the first line print $m$ ($0 \le m \le 5 \cdot n$)&nbsp;！ the number of swaps to perform.</p><p>Each of the following $m$ lines should contain integers $a_i, b_i$ ($1 \le a_i, b_i \le n$, $|a_i - b_i| \ge \frac{n}{2}$)&nbsp;！ the indices that should be swapped in the corresponding swap.</p><p>Note that there is no need to minimize the number of operations. We can show that an answer always exists.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$, $n$ is even)&nbsp;！ the length of the permutation. </p><p>The second line contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;！ the given permutation.</p>

## Output

<p>On the first line print $m$ ($0 \le m \le 5 \cdot n$)&nbsp;！ the number of swaps to perform.</p><p>Each of the following $m$ lines should contain integers $a_i, b_i$ ($1 \le a_i, b_i \le n$, $|a_i - b_i| \ge \frac{n}{2}$)&nbsp;！ the indices that should be swapped in the corresponding swap.</p><p>Note that there is no need to minimize the number of operations. We can show that an answer always exists.</p>

## Samples

```input1
2
2 1
```

```output1
1
1 2
```






```input2
4
3 4 1 2
```

```output2
4
1 4
1 4
1 3
2 4
```






```input3
6
2 5 3 1 4 6
```

```output3
3
1 5
2 5
1 4
```




## Note

<p>In the first example, when one swap elements on positions $1$ and $2$, the array becomes sorted.</p><p>In the second example, pay attention that there is no need to minimize number of swaps.</p><p>In the third example, after swapping elements on positions $1$ and $5$ the array becomes: $[4, 5, 3, 1, 2, 6]$. After swapping elements on positions $2$ and $5$ the array becomes $[4, 2, 3, 1, 5, 6]$ and finally after swapping elements on positions $1$ and $4$ the array becomes sorted: $[1, 2, 3, 4, 5, 6]$.</p>
