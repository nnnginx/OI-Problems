## Description

<div><p>You are the proud owner of an infinitely large grid of lightbulbs, represented by a <a href="https://en.wikipedia.org/wiki/Cartesian_coordinate_system">Cartesian coordinate system</a>. Initially, all of the lightbulbs are turned off, except for one lightbulb, where you buried your proudest treasure.</p><p>In order to hide your treasure's position, you perform the following operation an arbitrary number of times (possibly zero):</p><ul> <li> Choose two <span class="tex-font-style-bf">integer</span> numbers $x$ and $y$, and switch the state of the $4$ lightbulbs at $(x, y)$, $(x, y + 1)$, $(x + 1, y - 1)$, and $(x + 1, y)$. In other words, for each lightbulb, turn it on if it was off, and turn it off if it was on. Note that there are <span class="tex-font-style-bf">no constraints</span> on $x$ and $y$. </li></ul><p>In the end, there are $n$ lightbulbs turned on at coordinates $(x_1, y_1), (x_2, y_2), \ldots, (x_n, y_n)$. Unfortunately, you have already forgotten where you buried your treasure, so now you have to figure out one possible position of the treasure. Good luck!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of lightbulbs that are on.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($\color{red}{-10^8} \le x_i, y_i \le \color{red}{10^8}$)&nbsp;！ the coordinates of the $i$-th lightbulb. It is guaranteed that all coordinates are distinct.</p><p><span class="tex-font-style-bf">Additional constraint</span>: There exists at least one position $(s, t)$ ($\color{red}{-10^9} \le s, t \le \color{red}{10^9}$), such that if the lightbulb at position $(s, t)$ is initially turned on, then after performing an arbitrary number of operations (possibly zero), we will get the given configuration of lightbulbs.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two integers $s$ and $t$ ($-10^9 \le s, t \le 10^9$)&nbsp;！ one possible position of the buried treasure. If there are multiple solutions, print any of them.</p><p><span class="tex-font-style-bf">For this problem, hacks are disabled.</span></p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of lightbulbs that are on.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($\color{red}{-10^8} \le x_i, y_i \le \color{red}{10^8}$)&nbsp;！ the coordinates of the $i$-th lightbulb. It is guaranteed that all coordinates are distinct.</p><p><span class="tex-font-style-bf">Additional constraint</span>: There exists at least one position $(s, t)$ ($\color{red}{-10^9} \le s, t \le \color{red}{10^9}$), such that if the lightbulb at position $(s, t)$ is initially turned on, then after performing an arbitrary number of operations (possibly zero), we will get the given configuration of lightbulbs.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two integers $s$ and $t$ ($-10^9 \le s, t \le 10^9$)&nbsp;！ one possible position of the buried treasure. If there are multiple solutions, print any of them.</p><p><span class="tex-font-style-bf">For this problem, hacks are disabled.</span></p>





```input1|2,3,8,9,10,11,12,13,14,15
4
1
2 3
3
-2 -1
-1 -2
-1 -3
7
7 26
6 27
6 28
7 27
8 26
8 27
7 28
11
70 9
69 8
69 0
73 5
70 -1
70 5
71 7
70 4
73 4
71 3
72 3
```




```output1
2 3
-2 -2
7 27
72 7
```



## Note

<p>For the first test case, one possible scenario is that you hid your treasure at position $(2, 3)$. Then, you did not perform any operations.</p><p>In the end, only the lightbulb at $(2, 3)$ is turned on.</p><p>For the second test case, one possible scenario is that you hid your treasure at position $(-2, -2)$. Then, you performed $1$ operation with $x = -2$, $y = -2$.</p><p>The operation switches the state of the $4$ lightbulbs at $(-2, -2)$, $(-2, -1)$, $(-1, -3)$, and $(-1, -2)$.</p><p>In the end, the lightbulbs at $(-2, -1)$, $(-1, -2)$, and $(-1, -3)$ are turned on.</p>
