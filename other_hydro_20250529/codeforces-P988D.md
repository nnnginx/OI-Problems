## Description

<div><p>There are $n$ distinct points on a coordinate line, the coordinate of $i$-th point equals to $x_i$. Choose a subset of the given set of points such that the distance between each pair of points in a subset is an integral power of two. It is necessary to consider each pair of points, not only adjacent. Note that any subset containing one element satisfies the condition above. Among all these subsets, choose a subset with maximum possible size.</p><p>In other words, you have to choose the maximum possible number of points $x_{i_1}, x_{i_2}, \dots, x_{i_m}$ such that for each pair $x_{i_j}$, $x_{i_k}$ it is true that $|x_{i_j} - x_{i_k}| = 2^d$ where $d$ is some non-negative integer number (not necessarily the same for each pair of points).</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of points.</p><p>The second line contains $n$ pairwise distinct integers $x_1, x_2, \dots, x_n$ ($-10^9 \le x_i \le 10^9$) ！ the coordinates of points.</p></div><div class="output-specification"><p>In the first line print $m$ ！ the maximum possible number of points in a subset that satisfies the conditions described above.</p><p>In the second line print $m$ integers ！ the coordinates of points in the subset you have chosen.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of points.</p><p>The second line contains $n$ pairwise distinct integers $x_1, x_2, \dots, x_n$ ($-10^9 \le x_i \le 10^9$) ！ the coordinates of points.</p>

## Output

<p>In the first line print $m$ ！ the maximum possible number of points in a subset that satisfies the conditions described above.</p><p>In the second line print $m$ integers ！ the coordinates of points in the subset you have chosen.</p><p>If there are multiple answers, print any of them.</p>

## Samples

```input1
6
3 5 4 7 10 12

```

```output1
3
7 3 5
```






```input2
5
-1 2 5 8 11

```

```output2
1
8

```




## Note

<p>In the first example the answer is $[7, 3, 5]$. Note, that $|7-3|=4=2^2$, $|7-5|=2=2^1$ and $|3-5|=2=2^1$. You can't find a subset having more points satisfying the required property.</p>
