## Description

<div><p>You are given a <span class="tex-font-style-it">complete directed</span> graph $K_n$ with $n$ vertices: each pair of vertices $u \neq v$ in $K_n$ have both directed edges $(u, v)$ and $(v, u)$; there are no self-loops.</p><p>You should find such a cycle in $K_n$ that visits every directed edge exactly once (allowing for revisiting vertices).</p><p>We can write such cycle as a list of $n(n - 1) + 1$ vertices $v_1, v_2, v_3, \dots, v_{n(n - 1) - 1}, v_{n(n - 1)}, v_{n(n - 1) + 1} = v_1$ ！ a visiting order, where each $(v_i, v_{i + 1})$ occurs exactly once.</p><p>Find the <span class="tex-font-style-bf">lexicographically smallest</span> such cycle. It's not hard to prove that the cycle always exists.</p><p>Since the answer can be too large print its $[l, r]$ segment, in other words, $v_l, v_{l + 1}, \dots, v_r$.</p></div><div class="input-specification"><p>The first line contains the single integer $T$ ($1 \le T \le 100$) ！ the number of test cases.</p><p>Next $T$ lines contain test cases ！ one per line. The first and only line of each test case contains three integers $n$, $l$ and $r$ ($2 \le n \le 10^5$, $1 \le l \le r \le n(n - 1) + 1$, $r - l + 1 \le 10^5$) ！ the number of vertices in $K_n$, and segment of the cycle to print.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$ and the total sum of $r - l + 1$ doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the segment $v_l, v_{l + 1}, \dots, v_r$ of the lexicographically smallest cycle that visits every edge exactly once.</p></div>

## Input

<p>The first line contains the single integer $T$ ($1 \le T \le 100$) ！ the number of test cases.</p><p>Next $T$ lines contain test cases ！ one per line. The first and only line of each test case contains three integers $n$, $l$ and $r$ ($2 \le n \le 10^5$, $1 \le l \le r \le n(n - 1) + 1$, $r - l + 1 \le 10^5$) ！ the number of vertices in $K_n$, and segment of the cycle to print.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$ and the total sum of $r - l + 1$ doesn't exceed $10^5$.</p>

## Output

<p>For each test case print the segment $v_l, v_{l + 1}, \dots, v_r$ of the lexicographically smallest cycle that visits every edge exactly once.</p>

## Samples

```input1
3
2 1 3
3 3 6
99995 9998900031 9998900031
```

```output1
1 2 1 
1 3 2 3 
1
```




## Note

<p>In the second test case, the lexicographically minimum cycle looks like: $1, 2, 1, 3, 2, 3, 1$.</p><p>In the third test case, it's quite obvious that the cycle should start and end in vertex $1$.</p>
