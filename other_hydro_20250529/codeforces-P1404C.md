## Description

<div><p>Let $a_1, \ldots, a_n$ be an array of $n$ positive integers. In one operation, you can choose an index $i$ such that $a_i = i$, and remove $a_i$ from the array (after the removal, the remaining parts are concatenated).</p><p>The weight of $a$ is defined as the maximum number of elements you can remove.</p><p>You must answer $q$ independent queries $(x, y)$: after replacing the $x$ first elements of $a$ and the $y$ last elements of $a$ by $n+1$ (making them impossible to remove), what would be the weight of $a$?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$) &nbsp;！ the length of the array and the number of queries.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \leq a_i \leq n$)&nbsp;！ elements of the array.</p><p>The $i$-th of the next $q$ lines contains two integers $x$ and $y$ ($x, y \ge 0$ and $x+y &lt; n$).</p></div><div class="output-specification"><p>Print $q$ lines, $i$-th line should contain a single integer &nbsp;！ the answer to the $i$-th query.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$) &nbsp;！ the length of the array and the number of queries.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \leq a_i \leq n$)&nbsp;！ elements of the array.</p><p>The $i$-th of the next $q$ lines contains two integers $x$ and $y$ ($x, y \ge 0$ and $x+y &lt; n$).</p>

## Output

<p>Print $q$ lines, $i$-th line should contain a single integer &nbsp;！ the answer to the $i$-th query.</p>

## Samples

```input1
13 5
2 2 3 9 5 4 6 5 7 8 3 11 13
3 1
0 0
2 4
5 0
0 12
```

```output1
5
11
6
1
0
```






```input2
5 2
1 4 1 2 4
0 0
1 0
```

```output2
2
0
```




## Note

<p>Explanation of the first query:</p><p>After making first $x = 3$ and last $y = 1$ elements impossible to remove, $a$ becomes $[\times, \times, \times, 9, 5, 4, 6, 5, 7, 8, 3, 11, \times]$ (we represent $14$ as $\times$ for clarity).</p><p>Here is a strategy that removes $5$ elements (the element removed is colored in red):</p><ul> <li> $[\times, \times, \times, 9, \color{red}{5}, 4, 6, 5, 7, 8, 3, 11, \times]$ </li><li> $[\times, \times, \times, 9, 4, 6, 5, 7, 8, 3, \color{red}{11}, \times]$ </li><li> $[\times, \times, \times, 9, 4, \color{red}{6}, 5, 7, 8, 3, \times]$ </li><li> $[\times, \times, \times, 9, 4, 5, 7, \color{red}{8}, 3, \times]$ </li><li> $[\times, \times, \times, 9, 4, 5, \color{red}{7}, 3, \times]$ </li><li> $[\times, \times, \times, 9, 4, 5, 3, \times]$ (final state) </li></ul><p>It is impossible to remove more than $5$ elements, hence the weight is $5$.</p>
