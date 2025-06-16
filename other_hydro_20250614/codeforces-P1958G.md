## Description

<div><p>Consider a segment of an OX axis from $1$ to $n$. There are $k$ observation towers on this segment.</p><p>Each tower has two parameters&nbsp;！ the coordinate $x_i$ and the height $h_i$. The coordinates of all towers are distinct. From tower $i$, you can see point $j$ if $|x_i - j| \le h_i$ (where $|a|$ is an absolute value of $a$).</p><p>You can increase the height of any tower by $1$ for one coin. The height of each tower can be increased any number of times (including zero).</p><p>You need to process $q$ independent queries. In the $i$-th query, two different points $l$ and $r$ are given. You need to calculate the minimum number of coins required to be able to see both of these points (from one tower or from different towers).</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $1 \le k \le n$)&nbsp;！ the length of the segment of an OX axis and the number of observation towers.</p><p>The second line contains $k$ integers $x_1, x_2, \dots, x_k$ ($1 \le x_i \le n$)&nbsp;！ the coordinates of the observation towers. The coordinates of all towers are distinct.</p><p>The third line contains $k$ integers $h_1, h_2, \dots, h_k$ ($0 \le h_i \le n$)&nbsp;！ the heights of the observation towers.</p><p>The fourth line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$)&nbsp;！ the description of the next query.</p></div><div class="output-specification"><p>For each query, output a single integer&nbsp;！ the minimum number of coins required to be able to see both points (from one tower or from different towers).</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $1 \le k \le n$)&nbsp;！ the length of the segment of an OX axis and the number of observation towers.</p><p>The second line contains $k$ integers $x_1, x_2, \dots, x_k$ ($1 \le x_i \le n$)&nbsp;！ the coordinates of the observation towers. The coordinates of all towers are distinct.</p><p>The third line contains $k$ integers $h_1, h_2, \dots, h_k$ ($0 \le h_i \le n$)&nbsp;！ the heights of the observation towers.</p><p>The fourth line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$)&nbsp;！ the description of the next query.</p>

## Output

<p>For each query, output a single integer&nbsp;！ the minimum number of coins required to be able to see both points (from one tower or from different towers).</p>





```input1|
20 3
2 15 10
6 2 0
3
1 20
10 11
3 4
```




```input2|
10 2
2 9
1 2
3
4 5
5 6
1 10
```




```output1
3 1 0
```




```output2
2 2 0
```


