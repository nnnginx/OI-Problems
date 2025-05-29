## Description

<div><p>In Bobritto Bandito's home town of residence, there are an infinite number of houses on an infinite number line, with houses at $\ldots, -2, -1, 0, 1, 2, \ldots$. On day $0$, he started a plague by giving an infection to the unfortunate residents of house $0$. Each succeeding day, the plague spreads to <span class="tex-font-style-bf">exactly one</span> healthy household that is next to an infected household. It can be shown that each day the infected houses form a continuous segment.</p><p>Let the segment starting at the $l$-th house and ending at the $r$-th house be denoted as $[l, r]$. You know that after $n$ days, the segment $[l, r]$ became infected. Find any such segment $[l', r']$ that could have been infected on the $m$-th day ($m \le n$).</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;¨C the number of independent test cases.</p><p>The only line of each test case contains four integers $n$, $m$, $l$, and $r$ ($1 \leq m\leq n \leq 2000, -n \leq l \leq 0 \leq r \leq n, r-l=n$).</p></div><div class="output-specification"><p>For each test case, output two integers $l'$ and $r'$ on a new line. If there are multiple solutions, output any.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;¨C the number of independent test cases.</p><p>The only line of each test case contains four integers $n$, $m$, $l$, and $r$ ($1 \leq m\leq n \leq 2000, -n \leq l \leq 0 \leq r \leq n, r-l=n$).</p>

## Output

<p>For each test case, output two integers $l'$ and $r'$ on a new line. If there are multiple solutions, output any.</p>





```input1|2,4
4
4 2 -2 2
4 1 0 4
3 3 -1 2
9 8 -6 3
```




```output1
-1 1
0 1
-1 2
-5 3
```



## Note

<p>In the first test case, it is possible that on the $1$-st, $2$-nd, and $3$-rd days the interval of houses affected is $[-1,0]$, $[-1,1]$, $[-2,1]$. Therefore, $[-1,1]$ is a valid output.</p>
