## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that in this version $k \le 10^{12}$. You can make hacks only if both versions of the problem are solved.</span></p><p>Given a $w \times h$ rectangle on the $Oxy$ plane, with points $(0, 0)$ at the bottom-left and $(w, h)$ at the top-right of the rectangle.</p><p>You also have a robot initially at point $(0, 0)$ and a script $s$ of $n$ characters. Each character is either <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span>, or <span class="tex-font-style-tt">D</span>, which tells the robot to move left, right, up, or down respectively.</p><p>The robot can only move inside the rectangle; otherwise, it will change the script $s$ as follows:</p><ul> <li> If it tries to move outside a vertical border, it changes all <span class="tex-font-style-tt">L</span> characters to <span class="tex-font-style-tt">R</span>'s (and vice versa, all <span class="tex-font-style-tt">R</span>'s to <span class="tex-font-style-tt">L</span>'s). </li><li> If it tries to move outside a horizontal border, it changes all <span class="tex-font-style-tt">U</span> characters to <span class="tex-font-style-tt">D</span>'s (and vice versa, all <span class="tex-font-style-tt">D</span>'s to <span class="tex-font-style-tt">U</span>'s). </li></ul><p>Then, it will execute the changed script starting from the character which it couldn't execute.</p><center> <img class="tex-graphics" src="./34811/file/zQouKhFU.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> <span class="tex-font-size-normal">An example of the robot's movement process, $s = \texttt{"ULULURD"}$</span> </center><p>The script $s$ will be executed for $k$ times continuously. All changes to the string $s$ will be retained even when it is repeated. During this process, how many times will the robot move to the point $(0, 0)$ in total? <span class="tex-font-style-bf">Note that the initial position does NOT count</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains four integers $n$, $k$, $w$, and $h$ ($1 \le n, w, h \le 10^6$; $1 \le k \le 10^{12}$).</p><p>The second line contains a single string $s$ of size $n$ ($s_i \in \{\texttt{L}, \texttt{R}, \texttt{U}, \texttt{D}\}$)&nbsp;！ the script to be executed.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the number of times the robot reaches $(0, 0)$ when executing script $s$ for $k$ times continuously.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains four integers $n$, $k$, $w$, and $h$ ($1 \le n, w, h \le 10^6$; $1 \le k \le 10^{12}$).</p><p>The second line contains a single string $s$ of size $n$ ($s_i \in \{\texttt{L}, \texttt{R}, \texttt{U}, \texttt{D}\}$)&nbsp;！ the script to be executed.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the number of times the robot reaches $(0, 0)$ when executing script $s$ for $k$ times continuously.</p>





```input1|2,3,6,7,10,11
6
2 4 2 2
UR
4 2 1 1
LLDD
6 3 3 1
RLRRRL
5 6 3 3
RUURD
7 5 3 4
RRDLUUU
7 123456789999 3 2
ULULURD
```




```output1
1
4
3
1
1
41152263332
```



## Note

<p>In the first test case, the robot only moves up and right for the first two executions. After that, it occupies the position $(2, 2)$. For the next two executions, it moves down and left and finishes at $(0, 0)$. So the answer is $1$.</p><p>In the second test case, each time executing the script the robot visits the origin twice. And since $k=2$, it visits the origin $2 \cdot 2 = 4$ times overall. </p><center> <img class="tex-graphics" src="./34811/file/IWwXnjLe.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>In the third test case, the visualization is shown as below: </p><center> <img class="tex-graphics" src="./34811/file/Wo7W9kpd.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center>
