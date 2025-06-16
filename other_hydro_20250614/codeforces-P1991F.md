## Description

<div><p>You are given $n$ sticks, numbered from $1$ to $n$. The length of the $i$-th stick is $a_i$.</p><p>You need to answer $q$ queries. In each query, you are given two integers $l$ and $r$ ($1 \le l &lt; r \le n$, $r - l + 1 \ge 6$). Determine whether it is possible to choose $6$ <span class="tex-font-style-bf">distinct</span> sticks from the sticks numbered $l$ to $r$, to form $2$ <span class="tex-font-style-bf">non-degenerate</span> triangles$^{\text{∗}}$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A triangle with side lengths $a$, $b$, and $c$ is called non-degenerate if: </p><ul> <li> $a &lt; b + c$, </li><li> $b &lt; a + c$, and </li><li> $c &lt; a + b$. </li></ul></div></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($6 \le n \le 10^5$, $1 \le q \le 10^5$)&nbsp;— the number of sticks and the number of queries respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— $a_i$ denotes the length of the $i$-th stick.</p><p>Each of the following $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$, $r - l + 1 \ge 6$)&nbsp;— the parameters of each query.</p></div><div class="output-specification"><p>For each query, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to form $2$ triangles, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($6 \le n \le 10^5$, $1 \le q \le 10^5$)&nbsp;— the number of sticks and the number of queries respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— $a_i$ denotes the length of the $i$-th stick.</p><p>Each of the following $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$, $r - l + 1 \ge 6$)&nbsp;— the parameters of each query.</p>

## Output

<p>For each query, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to form $2$ triangles, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|3,5,7
10 5
5 2 2 10 4 10 6 1 5 3
1 6
2 7
2 8
5 10
4 10
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the first query, the lengths of the sticks are $[5, 2, 2, 10, 4, 10]$. Two sets of sticks $[2, 4, 5]$ and $[2, 10, 10]$ can be selected to form $2$ non-degenerate triangles.</p><p>In the second query, the lengths of the sticks are $[2, 2, 10, 4, 10, 6]$. It can be shown that it is impossible to form $2$ non-degenerate triangles.</p><p>In the third query, the lengths of the sticks are $[2, 2, 10, 4, 10, 6, 1]$. Two sets of sticks $[1, 2, 2]$ and $[4, 10, 10]$ can be selected to form $2$ non-degenerate triangles.</p><p>In the fourth query, the lengths of the sticks are $[4, 10, 6, 1, 5, 3]$. It can be shown that it is impossible to form $2$ non-degenerate triangles.</p><p>In the fifth query, the lengths of the sticks are $[10, 4, 10, 6, 1, 5, 3]$. Two sets of sticks $[1, 10, 10]$ and $[3, 4, 5]$ can be selected to form $2$ non-degenerate triangles.</p>
