## Description

<div><p>For a vector $\vec{v} = (x, y)$, define $|v| = \sqrt{x^2 + y^2}$.</p><p>Allen had a bit too much to drink at the bar, which is at the origin. There are $n$ vectors $\vec{v_1}, \vec{v_2}, \cdots, \vec{v_n}$. Allen will make $n$ moves. As Allen's sense of direction is impaired, during the $i$-th move he will either move in the direction $\vec{v_i}$ or $-\vec{v_i}$. In other words, if his position is currently $p = (x, y)$, he will either move to $p + \vec{v_i}$ or $p - \vec{v_i}$.</p><p>Allen doesn't want to wander too far from home (which happens to also be the bar). You need to help him figure out a sequence of moves (a sequence of signs for the vectors) such that his final position $p$ satisfies $|p| \le 1.5 \cdot 10^6$ so that he can stay safe.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the number of moves.</p><p>Each of the following lines contains two space-separated integers $x_i$ and $y_i$, meaning that $\vec{v_i} = (x_i, y_i)$. We have that $|v_i| \le 10^6$ for all $i$.</p></div><div class="output-specification"><p>Output a single line containing $n$ integers $c_1, c_2, \cdots, c_n$, each of which is either $1$ or $-1$. Your solution is correct if the value of $p = \sum_{i = 1}^n c_i \vec{v_i}$, satisfies $|p| \le 1.5 \cdot 10^6$.</p><p>It can be shown that a solution always exists under the given constraints.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the number of moves.</p><p>Each of the following lines contains two space-separated integers $x_i$ and $y_i$, meaning that $\vec{v_i} = (x_i, y_i)$. We have that $|v_i| \le 10^6$ for all $i$.</p>

## Output

<p>Output a single line containing $n$ integers $c_1, c_2, \cdots, c_n$, each of which is either $1$ or $-1$. Your solution is correct if the value of $p = \sum_{i = 1}^n c_i \vec{v_i}$, satisfies $|p| \le 1.5 \cdot 10^6$.</p><p>It can be shown that a solution always exists under the given constraints.</p>

## Samples

```input1
3
999999 0
0 999999
999999 0

```

```output1
1 1 -1 

```






```input2
1
-824590 246031

```

```output2
1 

```






```input3
8
-67761 603277
640586 -396671
46147 -122580
569609 -2112
400 914208
131792 309779
-850150 -486293
5272 721899

```

```output3
1 1 1 1 1 1 1 -1 

```



