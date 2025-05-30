## Description

<div><p>Ray lost his array and needs to find it by asking Omkar. Omkar is willing to disclose that the array has the following qualities:</p><ol> <li> The array has $n$ ($1 \le n \le 2 \cdot 10^5$) elements. </li><li> Every element in the array $a_i$ is an integer in the range $1 \le a_i \le 10^9.$ </li><li> The array is sorted in nondecreasing order. </li></ol><p>Ray is allowed to send Omkar a series of queries. A query consists of two integers, $l$ and $r$ such that $1 \le l \le r \le n$. Omkar will respond with two integers, $x$ and $f$. $x$ is the mode of the subarray from index $l$ to index $r$ inclusive. The mode of an array is defined by the number that appears the most frequently. If there are multiple numbers that appear the most number of times, the smallest such number is considered to be the mode. $f$ is the amount of times that $x$ appears in the queried subarray.</p><p>The array has $k$ ($1 \le k \le \min(25000,n)$) distinct elements. However, due to Ray's sins, Omkar will not tell Ray what $k$ is. Ray is allowed to send at most $4k$ queries.</p><p>Help Ray find his lost array.</p></div><div class="input-specification"><p>The only line of the input contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$), which equals to the length of the array that you are trying to find.</p></div><div><h2>Interaction</h2><p>The interaction starts with reading $n$.</p><p>Then you can make one type of query:</p><ul> <li> "$? \enspace l \enspace r$" ($1 \le l \le r \le n$) where $l$ and $r$ are the bounds of the subarray that you wish to query. </li></ul><p>The answer to each query will be in the form "$x \enspace f$" where $x$ is the mode of the subarray and $f$ is the number of times $x$ appears in the subarray.</p><ul> <li> $x$ satisfies ($1 \leq x \leq 10^9$). </li><li> $f$ satisfies ($1 \leq f \leq r-l+1$). </li><li> If you make more than $4k$ queries or violate the number range in the query, you will get an output "<span class="tex-font-style-tt">-1</span>." </li><li> If you terminate after receiving the response "$-1$", you will get the "<span class="tex-font-style-tt">Wrong answer</span>" verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream. </li></ul><p>To output your answer, print:</p><ul> <li> "$! \enspace a_1 \enspace a_2 \enspace \ldots \enspace a_{n-1} \enspace a_n$" which is an exclamation point followed by the array with a space between every element. </li></ul><p>And quit after that. This query is not counted towards the $4k$ queries limit.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hack Format</span></p><p>To hack, output $1$ integer on the first line, $n$ ($1 \le n \le 2 \cdot 10^5$). On the second line output $n$ integers $a_1, a_2, \ldots, a_{n-1}, a_n$ separated by a space such that there are at most $25000$ distinct numbers and $a_j \le a_{j+1}$ for all $j$ from $1$ to $n-1$.</p></div>

## Input

<p>The only line of the input contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$), which equals to the length of the array that you are trying to find.</p>

## Samples

```input1
6

2 2

2 2

3 2

2 1
```

```output1
? 1 6

? 1 3

? 4 6

? 3 4

! 1 2 2 3 3 4
```




## Note

<p>The first query is $l=1$ and $r=6$. The mode is $2$, and $2$ appears $2$ times, so $x=2$ and $f=2$. Note that $3$ also appears two times, but $2$ is outputted because $2$ is smaller.</p><p>The second query is $l=1$ and $r=3$. The mode is $2$ and $2$ appears twice in the subarray with indices $[1,3]$.</p><p>The third query is $l=4$ and $r=6$. The mode is $3$ and $3$ appears twice in the subarray with indices $[4,6]$.</p><p>The fourth query is $l=3$ and $r=4$. The mode is $2$, which appears once in the subarray with indices $[3,4]$. Note that $3$ also appears once in that range, but $2$ is smaller than $3$.</p>
