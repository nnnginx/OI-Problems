## Description

<div><p>Bob has a grid with $3$ rows and $n$ columns, each of which contains either $a_i$ or $-a_i$ for some integer $1 \leq i \leq n$. For example, one possible grid for $n=4$ is shown below:</p><p>$$\begin{bmatrix} a_1 &amp; -a_2 &amp; -a_3 &amp; -a_2 \\ -a_4 &amp; a_4 &amp; -a_1 &amp; -a_3 \\ a_1 &amp; a_2 &amp; -a_2 &amp; a_4 \end{bmatrix}$$</p><p>Alice and Bob play a game as follows: </p><ul> <li> Bob shows Alice his grid. </li><li> Alice gives Bob an array $a_1, a_2, \dots, a_n$ of her choosing, <span class="tex-font-style-bf">whose elements are all $\mathbf{-1}$ or $\mathbf{1}$</span>. </li><li> Bob substitutes these values into his grid to make a grid of $-1$s and $1$s. </li><li> Bob <span class="tex-font-style-bf">sorts</span> the elements of each column in non-decreasing order. </li><li> Alice wins if all the elements in the middle row are $1$; otherwise, Bob wins. </li></ul><p>For example, suppose Alice gives Bob the array $[1, -1, -1, 1]$ for the grid above. Then the following will happen (colors are added for clarity):</p><p>$$\begin{bmatrix} \color{red}{a_1} &amp; \color{green}{-a_2} &amp; \color{blue}{-a_3} &amp; \color{green}{-a_2} \\ -a_4 &amp; a_4 &amp; \color{red}{-a_1} &amp; \color{blue}{-a_3} \\ \color{red}{a_1} &amp; \color{green}{a_2} &amp; \color{green}{-a_2} &amp; a_4 \end{bmatrix} \xrightarrow{[\color{red}{1},\color{green}{-1},\color{blue}{-1},1]} \begin{bmatrix} \color{red}{1} &amp; \color{green}{1} &amp; \color{blue}{1} &amp; \color{green}{1} \\ -1 &amp; 1 &amp; \color{red}{-1} &amp; \color{blue}{1} \\ \color{red}{1} &amp; \color{green}{-1} &amp; \color{green}{1} &amp; 1 \end{bmatrix} \xrightarrow{\text{sort each column}} \begin{bmatrix} -1 &amp; -1 &amp; -1 &amp; 1 \\ \mathbf{1} &amp; \mathbf{1} &amp; \mathbf{1} &amp; \mathbf{1} \\ 1 &amp; 1 &amp; 1 &amp; 1 \\ \end{bmatrix}\,. $$ Since the middle row is all $1$, Alice wins.</p><p>Given Bob's grid, determine whether or not Alice can choose the array $a$ to win the game.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 500$)&nbsp;！ the number of columns of Bob's grid.</p><p>The next three lines each contain $n$ integers, the $i$-th of which contains $g_{i,1}, g_{i,2}, \dots, g_{i,n}$ ($-n \leq g_{i,j} \leq n$, $g_{i,j} \neq 0$), representing Bob's grid. </p><p>If cell $x &gt; 0$ is in the input, that cell in Bob's grid should contain $a_x$; if $x &lt; 0$ is in the input, that cell in Bob's grid should contain $-a_{-x}$. See the sample input and notes for a better understanding.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alice can win, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 500$)&nbsp;！ the number of columns of Bob's grid.</p><p>The next three lines each contain $n$ integers, the $i$-th of which contains $g_{i,1}, g_{i,2}, \dots, g_{i,n}$ ($-n \leq g_{i,j} \leq n$, $g_{i,j} \neq 0$), representing Bob's grid. </p><p>If cell $x &gt; 0$ is in the input, that cell in Bob's grid should contain $a_x$; if $x &lt; 0$ is in the input, that cell in Bob's grid should contain $-a_{-x}$. See the sample input and notes for a better understanding.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alice can win, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,4,5,10,11,12,13
4
4
1 -2 -3 -2
-4 4 -1 -3
1 2 -2 4
2
1 2
-1 -2
2 -2
5
1 2 3 4 5
-2 3 -4 -5 -1
3 -5 1 2 2
6
1 3 -6 2 5 2
1 3 -2 -3 -6 -5
-2 -1 -3 2 3 1
```




```output1
YES
NO
YES
NO
```



## Note

<p>The first test case is described in the statement.</p><p>In the second test case, Bob's grid is as follows:</p><p>$$\begin{bmatrix} a_1 &amp; a_2 \\ -a_1 &amp; -a_2 \\ a_2 &amp; -a_2 \end{bmatrix}$$</p><p>For the last column to have $1$ in the middle row when sorted, Alice must pick $a_2 = -1$. However, it is then impossible to choose $a_1$ such that the first column has $1$ in the middle when sorted. Thus, Alice cannot win.</p><p>In the third test case, Alice can pick $a = [1,1,1,1,1]$.</p>
