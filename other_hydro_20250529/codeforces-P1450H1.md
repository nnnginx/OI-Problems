## Description

<div><p><span class="tex-font-style-bf">The only difference between the two versions of the problem is that there are no updates in the easy version.</span></p><p>There are $n$ spools of thread placed on the rim of a circular table. The spools come in two types of thread: the first thread is black and the second thread is white.</p><p>For any two spools of the same color, you can attach them with a thread of that color in a straight line segment. Define a matching as a way to attach spools together so that each spool is attached to exactly one other spool.</p><p>Coloring is an assignment of colors (white and black) to the spools. A coloring is called <span class="tex-font-style-bf">valid</span> if it has at least one matching. That is if the number of black spools and the number of white spools are both even.</p><p>Given a matching, we can find the number of times some white thread intersects some black thread. We compute the number of pairs of differently colored threads that intersect instead of the number of intersection points, so one intersection point may be counted multiple times if different pairs of threads intersect at the same point. If $c$ is a valid coloring, let $f(c)$ denote the minimum number of such intersections out of all possible matchings.</p><center> <img class="tex-graphics" src="./31641/file/wpV8q1JV.png" style="max-width: 100.0%;max-height: 100.0%;"> The circle above is described by the coloring <span class="tex-font-style-tt">bwbbbwww</span>. After matching the spools as shown, there is one intersection between differently colored threads. It can be proven that it is the minimum possible, so $f(\text{bwbbbwww}) = 1$. </center><p>You are given a string $s$ representing an <span class="tex-font-style-bf">unfinished</span> coloring, with black, white, and uncolored spools. A coloring $c$ is called $s$-reachable if you can achieve it by assigning colors to the uncolored spools of $s$ without changing the others.</p><p>A coloring $c$ is chosen uniformly at random among all valid, $s$-reachable colorings. Compute the <a href="https://en.wikipedia.org/wiki/Expected_value">expected value</a> of $f(c)$. You should find it by modulo $998244353$.</p><p>We can show that the answer can be written in the form $\frac{p}{q}$ where $p$ and $q$ are relatively prime integers and $q\not\equiv 0\pmod{998244353}$. The answer by modulo $998244353$ is equal to $(p\cdot q^{-1})$ modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($2\le n\le 2\cdot 10^5$, $n$ is even, $m=0$) �� the number of spools and updates, respectively. There are no updates in the easy version, so it is always $0$.</p><p>The second line contains a string $s$ of length $n$ �� the unfinished coloring of the spools. The $i$-th character will be '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">b</span>', or '<span class="tex-font-style-tt">?</span>', describing if the $i$-th spool is white, black, or uncolored, respectively.</p><p>It is guaranteed there exists at least one uncolored spool.</p></div><div class="output-specification"><p>Print the expected value of $f(c)$ by modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($2\le n\le 2\cdot 10^5$, $n$ is even, $m=0$) �� the number of spools and updates, respectively. There are no updates in the easy version, so it is always $0$.</p><p>The second line contains a string $s$ of length $n$ �� the unfinished coloring of the spools. The $i$-th character will be '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">b</span>', or '<span class="tex-font-style-tt">?</span>', describing if the $i$-th spool is white, black, or uncolored, respectively.</p><p>It is guaranteed there exists at least one uncolored spool.</p>

## Output

<p>Print the expected value of $f(c)$ by modulo $998244353$.</p>

## Samples

```input1
8 0
bwbb?www
```

```output1
1
```






```input2
10 0
???ww?wb??
```

```output2
436731905
```






```input3
4 0
bw?b
```

```output3
0
```




## Note

<p>The first test corresponds closely to the image. Coloring '<span class="tex-font-style-tt">?</span>' as '<span class="tex-font-style-tt">w</span>' does not create a valid coloring because the number of black spools is odd. Then the only reachable valid coloring is '<span class="tex-font-style-tt">bwbbbwww</span>' and $f(\text{bwbbbwww}) = 1$, so the expected value is $1$.</p><p>It can be shown that the expected value for the second test is $\frac{9}{16}$.</p>
