## Description

<div><p>It turns out that the meaning of life is a permutation $p_1, p_2, \ldots, p_n$ of the integers $1, 2, \ldots, n$ ($2 \leq n \leq 100$). Omkar, having created all life, knows this permutation, and will allow you to figure it out using some queries.</p><p>A query consists of an array $a_1, a_2, \ldots, a_n$ of integers between $1$ and $n$. $a$ is <span class="tex-font-style-bf">not</span> required to be a permutation. Omkar will first compute the pairwise sum of $a$ and $p$, meaning that he will compute an array $s$ where $s_j = p_j + a_j$ for all $j = 1, 2, \ldots, n$. Then, he will find the smallest index $k$ such that $s_k$ occurs more than once in $s$, and answer with $k$. If there is no such index $k$, then he will answer with $0$.</p><p>You can perform at most $2n$ queries. Figure out the meaning of life $p$.</p></div><div><h2>Interaction</h2><p>Start the interaction by reading single integer $n$ ($2 \leq n \leq 100$) &nbsp;�� the length of the permutation $p$.</p><p>You can then make queries. A query consists of a single line "$? \enspace a_1 \enspace a_2 \enspace \ldots \enspace a_n$" ($1 \leq a_j \leq n$).</p><p>The answer to each query will be a single integer $k$ as described above ($0 \leq k \leq n$).</p><p>After making a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>To output your answer, print a single line "$! \enspace p_1 \enspace p_2 \enspace \ldots \enspace p_n$" then terminate.</p><p>You can make at most $2n$ queries. Outputting the answer does not count as a query.</p><p><span class="tex-font-style-bf">Hack Format</span></p><p>To hack, first output a line containing $n$ ($2 \leq n \leq 100$), then output another line containing the hidden permutation $p_1, p_2, \ldots, p_n$ of numbers from $1$ to $n$.</p></div>

## Samples

```input1
5

2

0

1
```

```output1
? 4 4 2 3 2

? 3 5 1 5 5

? 5 2 4 3 1

! 3 2 1 5 4
```




## Note

<p>In the sample, the hidden permutation $p$ is $[3, 2, 1, 5, 4]$. Three queries were made.</p><p>The first query is $a = [4, 4, 2, 3, 2]$. This yields $s = [3 + 4, 2 + 4, 1 + 2, 5 + 3, 4 + 2] = [7, 6, 3, 8, 6]$. $6$ is the only number that appears more than once, and it appears first at index $2$, making the answer to the query $2$.</p><p>The second query is $a = [3, 5, 1, 5, 5]$. This yields $s = [3 + 3, 2 + 5, 1 + 1, 5 + 5, 4 + 5] = [6, 7, 2, 10, 9]$. There are no numbers that appear more than once here, so the answer to the query is $0$.</p><p>The third query is $a = [5, 2, 4, 3, 1]$. This yields $s = [3 + 5, 2 + 2, 1 + 4, 5 + 3, 4 + 1] = [8, 4, 5, 8, 5]$. $5$ and $8$ both occur more than once here. $5$ first appears at index $3$, while $8$ first appears at index $1$, and $1 &lt; 3$, making the answer to the query $1$.</p><p>Note that the sample is only meant to provide an example of how the interaction works; it is not guaranteed that the above queries represent a correct strategy with which to determine the answer.</p>
