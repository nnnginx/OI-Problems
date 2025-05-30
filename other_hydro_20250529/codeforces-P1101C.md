## Description

<div><p>There are $n$ segments $[l_i, r_i]$ for $1 \le i \le n$. You should divide all segments into two <span class="tex-font-style-it">non-empty</span> groups in such way that there is no pair of segments from different groups which have at least one common point, or say that it's impossible to do it. Each segment should belong to exactly one group.</p><p>To optimize testing process you will be given multitest.</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 50000$) ！ the number of queries. Each query contains description of the set of segments. Queries are independent.</p><p>First line of each query contains single integer $n$ ($2 \le n \le 10^5$) ！ number of segments. It is guaranteed that $\sum{n}$ over all queries does not exceed $10^5$.</p><p>The next $n$ lines contains two integers $l_i$, $r_i$ per line ($1 \le l_i \le r_i \le 2 \cdot 10^5$) ！ the $i$-th segment.</p></div><div class="output-specification"><p>For each query print $n$ integers $t_1, t_2, \dots, t_n$ ($t_i \in \{1, 2\}$) ！ for each segment (in the same order as in the input) $t_i$ equals $1$ if the $i$-th segment will belongs to the first group and $2$ otherwise.</p><p>If there are multiple answers, you can print any of them. If there is no answer, print $-1$.</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 50000$) ！ the number of queries. Each query contains description of the set of segments. Queries are independent.</p><p>First line of each query contains single integer $n$ ($2 \le n \le 10^5$) ！ number of segments. It is guaranteed that $\sum{n}$ over all queries does not exceed $10^5$.</p><p>The next $n$ lines contains two integers $l_i$, $r_i$ per line ($1 \le l_i \le r_i \le 2 \cdot 10^5$) ！ the $i$-th segment.</p>

## Output

<p>For each query print $n$ integers $t_1, t_2, \dots, t_n$ ($t_i \in \{1, 2\}$) ！ for each segment (in the same order as in the input) $t_i$ equals $1$ if the $i$-th segment will belongs to the first group and $2$ otherwise.</p><p>If there are multiple answers, you can print any of them. If there is no answer, print $-1$.</p>

## Samples

```input1
3
2
5 5
2 3
3
3 5
2 3
2 3
3
3 3
4 4
5 5
```

```output1
2 1 
-1
1 1 2
```




## Note

<p>In the first query the first and the second segments should be in different groups, but exact numbers don't matter.</p><p>In the second query the third segment intersects with the first and the second segments, so they should be in the same group, but then the other group becomes empty, so answer is $-1$.</p><p>In the third query we can distribute segments in any way that makes groups non-empty, so any answer of $6$ possible is correct.</p>
