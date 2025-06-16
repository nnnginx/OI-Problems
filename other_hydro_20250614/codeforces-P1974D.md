## Description

<div><p>Let's imagine the surface of Mars as an infinite coordinate plane. Initially, the rover Perseverance-2 and the helicopter Ingenuity-2 are located at the point with coordinates $(0, 0)$. A set of instructions $s$ consisting of $n$ instructions of the following types was specially developed for them:</p><ul> <li> <span class="tex-font-style-tt">N</span>: move one meter north (from point $(x, y)$ to $(x, y + 1)$); </li><li> <span class="tex-font-style-tt">S</span>: move one meter south (from point $(x, y)$ to $(x, y - 1)$); </li><li> <span class="tex-font-style-tt">E</span>: move one meter east (from point $(x, y)$ to $(x + 1, y)$); </li><li> <span class="tex-font-style-tt">W</span>: move one meter west (from point $(x, y)$ to $(x - 1, y)$). </li></ul><p>Each instruction must be executed either by the rover or by the helicopter. Moreover, each device must execute <span class="tex-font-style-bf">at least one</span> instruction. Your task is to distribute the instructions in such a way that after executing all $n$ instructions, the helicopter and the rover end up at the same point, or determine that this is impossible.</p></div><div class="input-specification"><p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of instructions.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of the characters '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">S</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">W</span>'&nbsp;！ the sequence of instructions.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p></div><div class="output-specification"><p>For each test case, if the required distribution of instructions exists, output a string $p$ of length $n$ consisting of the characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">H</span>'. If the $i$-th operation should be executed by the rover, then $p_i=\text{R}$, if the $i$-th operation should be executed by the helicopter, then $p_i=\text{H}$. If there are multiple solutions, output any of them.</p><p>Otherwise, output <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of instructions.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of the characters '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">S</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">W</span>'&nbsp;！ the sequence of instructions.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p>

## Output

<p>For each test case, if the required distribution of instructions exists, output a string $p$ of length $n$ consisting of the characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">H</span>'. If the $i$-th operation should be executed by the rover, then $p_i=\text{R}$, if the $i$-th operation should be executed by the helicopter, then $p_i=\text{H}$. If there are multiple solutions, output any of them.</p><p>Otherwise, output <span class="tex-font-style-tt">NO</span>.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
6
NENSNE
3
WWW
6
NESSWS
2
SN
2
WE
4
SSNN
4
WESN
2
SS
4
EWNN
4
WEWE
```




```output1
RRHRRH
NO
HRRHRH
NO
NO
RHRH
RRHH
RH
RRRH
RRHH
```



## Note

<p>Let's consider the first example: the string $S = \texttt{NENSNE}$. One of the possible solutions, shown in the figure below, is $p = \texttt{RRHRRH}$, using which both the rover and the helicopter will end up one meter north and one meter east.</p><center> <img class="tex-graphics" src="./34671/file/zzTMNGXO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For <span class="tex-font-style-tt">WWW</span>, the solution is impossible.</p>
