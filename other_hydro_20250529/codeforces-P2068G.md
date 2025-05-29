## Description

<div><p>You are planning a hike in the Peneda-Ger那s National Park in the north of Portugal. The park takes its name from two of its highest peaks: Peneda (1340 m) and Ger那s (1545 m).</p><p>For this problem, the park is modelled as an infinite plane, where each position $(x, y)$, with $x, y$ being integers, has a specific altitude. The altitudes are defined by an $n \times n$ matrix $h$, which repeats periodically across the plane. Specifically, for any integers $a, b$ and $0 \leq x, y &lt; n$, the altitude at $(x + an, y + bn)$ is $h[x][y]$.</p><p>When you are at position $(x, y)$, you can move to any of the four adjacent positions: $(x, y+1)$, $(x+1, y)$, $(x, y-1)$, or $(x-1, y)$. The time required to move between two adjacent positions is $1 + \lvert \text{alt}_1 - \text{alt}_2 \rvert$, where $\text{alt}_1$ and $\text{alt}_2$ are the altitudes of the current and destination positions, respectively.</p><p>Initially, your position is $(0, 0)$. Compute the number of distinct positions you can reach within $10^{20}$ seconds. Your answer will be considered correct if its relative error is less than $10^{-6}$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2\le n\le 20$)〞the size of the matrix describing the altitudes.</p><p>The following $n$ lines contain $n$ integers each. The $(j+1)$-th number on the $(i+1)$-th of these lines is $h[i][j]$ ($0\le h[i][j] \le 1545$)〞the altitude of the position $(i, j)$.</p></div><div class="output-specification"><p>Print the number of distinct positions you can reach within $10^{20}$ seconds. Your answer will be considered correct if its relative error is less than $10^{-6}$.</p></div>

## Input

<p>The first line contains an integer $n$ ($2\le n\le 20$)〞the size of the matrix describing the altitudes.</p><p>The following $n$ lines contain $n$ integers each. The $(j+1)$-th number on the $(i+1)$-th of these lines is $h[i][j]$ ($0\le h[i][j] \le 1545$)〞the altitude of the position $(i, j)$.</p>

## Output

<p>Print the number of distinct positions you can reach within $10^{20}$ seconds. Your answer will be considered correct if its relative error is less than $10^{-6}$.</p>





```input1|
2
3 3
3 3
```




```input2|
3
0 0 0
0 1545 0
0 0 0
```




```input3|
4
0 1 2 3
5 6 7 4
10 11 8 9
15 12 13 14
```




```output1
2e+40
```




```output2
2e+40
```




```output3
1.524886878e+39
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, every position of the Peneda-Ger那s National Park has an altitude of $3$. Therefore, the time required to move between two adjacent positions is always equal to $1$ second.</p><p>In this case, one can show that a position $(x, y)$ is reachable within $10^{20}$ seconds if and only if $|x|+|y| \le 10^{20}$. One can compute that there exist $20\,000\,000\,000\,000\,000\,000\,200\,000\,000\,000\,000\,000\,001$ reachable positions and this number is approximated by $2\cdot 10^{40}$ with a relative error smaller than $10^{-6}$. The sample output shows $2\cdot 10^{40}$ as correct answer, but also the exact number of reachable positions would be a correct answer.</p><p>In the <span class="tex-font-style-bf">second sample</span>, every position $(x, y)$ of the Peneda-Ger那s National Park with $x-1$ and $y-1$ divisible by $3$ has an altitude of $1545$, while all the other positions have an altitude of $0$. For example, the time required to move between $(4, 10)$ and $(4, 9)$ is $1546$, while the time required to move between $(3, 2)$ and $(4, 2)$ is $1$. </p><p>The positions reachable in $2$ seconds are all positions $(x, y)$ with $|x|+|y|\le 2$ apart from $(1, 1)$ (which is on the peak). One can compute that there exist $19\,999\,999\,999\,999\,999\,931\,533\,333\,333\,333\,333\,863\,441$ reachable positions in $10^{20}$ seconds and this number is approximated by $2\cdot 10^{40}$ with a relative error smaller than $10^{-6}$. The sample output shows $2\cdot 10^{40}$ as correct answer, but also the exact number of reachable positions would be a correct answer.</p>
