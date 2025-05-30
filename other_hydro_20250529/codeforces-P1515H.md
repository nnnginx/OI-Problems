## Description

<div><p>Phoenix loves playing with bits&nbsp;！ specifically, by using the bitwise operations <span class="tex-font-style-tt">AND</span>, <span class="tex-font-style-tt">OR</span>, and <span class="tex-font-style-tt">XOR</span>. He has $n$ integers $a_1, a_2, \dots, a_n$, and will perform $q$ of the following queries:</p><ol> <li> replace all numbers $a_i$ where $l \le a_i \le r$ with $a_i$ <span class="tex-font-style-tt">AND</span> $x$; </li><li> replace all numbers $a_i$ where $l \le a_i \le r$ with $a_i$ <span class="tex-font-style-tt">OR</span> $x$; </li><li> replace all numbers $a_i$ where $l \le a_i \le r$ with $a_i$ <span class="tex-font-style-tt">XOR</span> $x$; </li><li> output how many <span class="tex-font-style-bf">distinct</span> integers $a_i$ where $l \le a_i \le r$. </li></ol><p>For each query, Phoenix is given $l$, $r$, and $x$. Note that he is considering the values of the numbers, not their indices.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le q \le 10^5$)&nbsp;！ the number of integers and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 2^{20}$)&nbsp;！ the integers that Phoenix starts with.</p><p>The next $q$ lines contain the queries. For each query, the first integer of each line is $t$ ($1 \le t \le 4$)&nbsp;！ the type of query.</p><p>If $t \in \{1, 2, 3\}$, then three integers $l_i$, $r_i$, and $x_i$ will follow ($0 \le l_i, r_i, x_i &lt; 2^{20}$; $l_i \le r_i$).</p><p>Otherwise, if $t=4$, two integers $l_i$ and $r_i$ will follow ($0 \le l_i \le r_i &lt; 2^{20}$).</p><p>It is guaranteed that there is at least one query where $t=4$.</p></div><div class="output-specification"><p>Print the answer for each query where $t=4$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le q \le 10^5$)&nbsp;！ the number of integers and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 2^{20}$)&nbsp;！ the integers that Phoenix starts with.</p><p>The next $q$ lines contain the queries. For each query, the first integer of each line is $t$ ($1 \le t \le 4$)&nbsp;！ the type of query.</p><p>If $t \in \{1, 2, 3\}$, then three integers $l_i$, $r_i$, and $x_i$ will follow ($0 \le l_i, r_i, x_i &lt; 2^{20}$; $l_i \le r_i$).</p><p>Otherwise, if $t=4$, two integers $l_i$ and $r_i$ will follow ($0 \le l_i \le r_i &lt; 2^{20}$).</p><p>It is guaranteed that there is at least one query where $t=4$.</p>

## Output

<p>Print the answer for each query where $t=4$.</p>

## Samples

```input1
5 6
5 4 3 2 1
1 2 3 2
4 2 5
3 2 5 3
4 1 6
2 1 1 8
4 8 10
```

```output1
3
2
1
```






```input2
6 7
6 0 2 3 2 7
1 0 4 3
2 6 8 4
4 0 7
3 2 5 3
1 0 1 2
4 0 3
4 2 7
```

```output2
5
1
2
```




## Note

<p>In the first example: </p><ul><li> For the first query, $2$ is replaced by $2$ <span class="tex-font-style-tt">AND</span> $2 = 2$ and $3$ is replaced with $3$ <span class="tex-font-style-tt">AND</span> $2 = 2$. The set of numbers is $\{1, 2, 4, 5\}$.</li><li> For the second query, there are $3$ distinct numbers between $2$ and $5$: $2$, $4$, and $5$.</li><li> For the third query, $2$ is replaced by $2$ <span class="tex-font-style-tt">XOR</span> $3 = 1$, $4$ is replaced by $4$ <span class="tex-font-style-tt">XOR</span> $3 = 7$, and $5$ is replaced by $5$ <span class="tex-font-style-tt">XOR</span> $3 = 6$. The set of numbers is $\{1, 6, 7\}$.</li><li> For the fourth query, there are $2$ distinct numbers between $1$ and $6$: $1$ and $6$.</li><li> For the fifth query, $1$ is replaced by $1$ <span class="tex-font-style-tt">OR</span> $8 = 9$. The set of numbers is $\{6, 7, 9\}$.</li><li> For the sixth query, there is one distinct number between $8$ and $10$: $9$. </li></ul>
