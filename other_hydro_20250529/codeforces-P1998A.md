## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">I couldn't think of a good title for this problem, so I decided to learn from LeetCode.</span></div><div class="epigraph-source">— Sun Tzu, <span class="tex-font-style-it">The Art of War</span></div></div><p>You are given three integers $x_c$, $y_c$, and $k$ ($-100 \leq x_c, y_c \leq 100$, $1 \leq k \leq 1000$). </p><p>You need to find $k$ <span class="tex-font-style-bf">distinct</span> points ($x_1, y_1$), ($x_2, y_2$), $\ldots$, ($x_k, y_k$), having integer coordinates, on the 2D coordinate plane such that: </p><ul> <li> their center$^{\text{∗}}$ is ($x_c, y_c$) </li><li> $-10^9 \leq x_i, y_i \leq 10^9$ for all $i$ from $1$ to $k$ </li></ul> <p>It can be proven that at least one set of $k$ distinct points always exists that satisfies these conditions.</p><div class="statement-footnote"><p>$^{\text{∗}}$The center of $k$ points ($x_1, y_1$), ($x_2, y_2$), $\ldots$, ($x_k, y_k$) is $\left( \frac{x_1 + x_2 + \ldots + x_k}{k}, \frac{y_1 + y_2 + \ldots + y_k}{k} \right)$.</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>Each test case contains three integers $x_c$, $y_c$, and $k$ ($-100 \leq x_c, y_c \leq 100$, $1 \leq k \leq 1000$)&nbsp;— the coordinates of the center and the number of distinct points you must output.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output $k$ lines, the $i$-th line containing two space separated integers, $x_i$ and $y_i$, ($-10^9 \leq x_i, y_i \leq 10^9$)&nbsp;— denoting the position of the $i$-th point.</p><p>If there are multiple answers, print any of them. It can be shown that a solution always exists under the given constraints.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>Each test case contains three integers $x_c$, $y_c$, and $k$ ($-100 \leq x_c, y_c \leq 100$, $1 \leq k \leq 1000$)&nbsp;— the coordinates of the center and the number of distinct points you must output.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output $k$ lines, the $i$-th line containing two space separated integers, $x_i$ and $y_i$, ($-10^9 \leq x_i, y_i \leq 10^9$)&nbsp;— denoting the position of the $i$-th point.</p><p>If there are multiple answers, print any of them. It can be shown that a solution always exists under the given constraints.</p>





```input1|2,4
4
10 10 1
0 0 3
-5 -8 8
4 -5 3
```




```output1
10 10
-1 -1
5 -1
-4 2
-6 -7
-5 -7
-4 -7
-4 -8
-4 -9
-5 -9
-6 -9
-6 -8
1000 -1000
-996 995
8 -10
```



## Note

<p>For the first test case, $\left( \frac{10}{1}, \frac{10}{1} \right) = (10, 10)$.</p><p>For the second test case, $\left( \frac{-1 + 5 - 4}{3}, \frac{-1 -1 + 2}{3} \right) = (0, 0)$.</p>
