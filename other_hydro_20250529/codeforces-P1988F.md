## Description

<div><p>For an array $u_1, u_2, \ldots, u_n$, define </p><ul> <li> a prefix maximum as an index $i$ such that $u_i&gt;u_j$ for all $j&lt;i$; </li><li> a suffix maximum as an index $i$ such that $u_i&gt;u_j$ for all $j&gt;i$; </li><li> an ascent as an index $i$ ($i&gt;1$) such that $u_i&gt;u_{i-1}$. </li></ul><p>You are given three cost arrays: $[a_1, a_2, \ldots, a_n]$, $[b_1, b_2, \ldots, b_n]$, and $[c_0, c_1, \ldots, c_{n-1}]$.</p><p>Define the <span class="tex-font-style-it">cost</span> of an array that has $x$ prefix maximums, $y$ suffix maximums, and $z$ ascents as $a_x\cdot b_y\cdot c_z$.</p><p>Let the sum of costs of all permutations of $1,2,\ldots,n$ be $f(n)$. Find $f(1)$, $f(2)$, ..., $f(n)$ modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1\le n\le 700$).</p><p>The second line contains $n$ integers $a_1,\ldots,a_n$ ($0\le a_i&lt;998\,244\,353$).</p><p>The third line contains $n$ integers $b_1,\ldots,b_n$ ($0\le b_i&lt;998\,244\,353$).</p><p>The fourth line contains $n$ integers $c_0,\ldots,c_{n-1}$ ($0\le c_i&lt;998\,244\,353$).</p></div><div class="output-specification"><p>Print $n$ integers: the $i$-th one is $f(i)$ modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1\le n\le 700$).</p><p>The second line contains $n$ integers $a_1,\ldots,a_n$ ($0\le a_i&lt;998\,244\,353$).</p><p>The third line contains $n$ integers $b_1,\ldots,b_n$ ($0\le b_i&lt;998\,244\,353$).</p><p>The fourth line contains $n$ integers $c_0,\ldots,c_{n-1}$ ($0\le c_i&lt;998\,244\,353$).</p>

## Output

<p>Print $n$ integers: the $i$-th one is $f(i)$ modulo $998\,244\,353$.</p>





```input1|
3
1 1 1
1 1 1
1 1 1
```




```input2|
3
1 2 3
2 3 1
3 1 2
```




```input3|
5
1 4 2 5 3
2 5 1 3 4
300000000 100000000 500000000 400000000 200000000
```




```output1
1 2 6
```




```output2
6 13 34
```




```output3
600000000 303511294 612289529 324650937 947905622
```



## Note

<p>In the second example:</p><ul> <li> Consider permutation $[1,2,3]$. Indices $1,2,3$ are prefix maximums. Index $3$ is the only suffix maximum. Indices $2,3$ are ascents. In conclusion, it has $3$ prefix maximums, $1$ suffix maximums, and $2$ ascents. Therefore, its cost is $a_3b_1c_2=12$. </li><li> Permutation $[1,3,2]$ has $2$ prefix maximums, $2$ suffix maximums, and $1$ ascent. Its cost is $6$. </li><li> Permutation $[2,1,3]$ has $2$ prefix maximums, $1$ suffix maximum, and $1$ ascent. Its cost is $4$. </li><li> Permutation $[2,3,1]$ has $2$ prefix maximums, $2$ suffix maximums, and $1$ ascent. Its cost is $6$. </li><li> Permutation $[3,1,2]$ has $1$ prefix maximum, $2$ suffix maximums, and $1$ ascent. Its cost is $3$. </li><li> Permutation $[3,2,1]$ has $1$ prefix maximum, $3$ suffix maximums, and $0$ ascents. Its cost is $3$. </li></ul><p>The sum of all permutations' costs is $34$, so $f(3)=34$.</p>
