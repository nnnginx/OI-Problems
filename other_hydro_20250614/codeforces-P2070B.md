## Description

<div><p>There is a robot on the coordinate line. Initially, the robot is located at the point $x$ ($x \ne 0$). The robot has a sequence of commands of length $n$ consisting of characters, where <span class="tex-font-style-tt">L</span> represents a move to the left by one unit (from point $p$ to point $(p-1)$) and <span class="tex-font-style-tt">R</span> represents a move to the right by one unit (from point $p$ to point $(p+1)$).</p><p>The robot starts executing this sequence of commands (one command per second, in the order they are presented). However, whenever the robot reaches the point $0$, the counter of executed commands is reset (i. e. it starts executing the entire sequence of commands from the very beginning). If the robot has completed all commands and is not at $0$, it stops.</p><p>Your task is to calculate how many times the robot will enter the point $0$ during the next $k$ seconds.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of a test case contains three integers $n$, $x$ and $k$ ($1 \le n \le 2 \cdot 10^5$; $-n \le x \le n$; $n \le k \le 10^{18}$).</p><p>The second line of a test case contains a string $s$ consisting of $n$ characters <span class="tex-font-style-tt">L</span> and/or <span class="tex-font-style-tt">R</span>.</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the number of times the robot will enter the point $0$ during the next $k$ seconds.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of a test case contains three integers $n$, $x$ and $k$ ($1 \le n \le 2 \cdot 10^5$; $-n \le x \le n$; $n \le k \le 10^{18}$).</p><p>The second line of a test case contains a string $s$ consisting of $n$ characters <span class="tex-font-style-tt">L</span> and/or <span class="tex-font-style-tt">R</span>.</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the number of times the robot will enter the point $0$ during the next $k$ seconds.</p>





```input1|2,3,6,7,10,11
6
3 2 6
LLR
2 -1 8
RL
4 -2 5
LRRR
5 3 7
LRRLL
1 1 1
L
3 -1 4846549234412827
RLR
```




```output1
1
4
1
0
1
2423274617206414
```



## Note

<p>In the first example, the robot moves as follows: $2 \rightarrow 1 \rightarrow \underline{0} \rightarrow -1 \rightarrow -2 \rightarrow -1$. The robot has completed all instructions from the sequence and is not at $0$. So it stops after $5$ seconds and the point $0$ is entered once.</p><p>In the second example, the robot moves as follows: $-1 \rightarrow \underline{0} \rightarrow 1 \rightarrow \underline{0} \rightarrow 1 \rightarrow \underline{0} \rightarrow 1 \rightarrow \underline{0} \rightarrow 1$. The robot worked $8$ seconds and the point $0$ is entered $4$ times.</p><p>In the third example, the robot moves as follows: $-2 \rightarrow -3 \rightarrow -2 \rightarrow -1 \rightarrow \underline{0} \rightarrow -1$. The robot worked $5$ seconds and the point $0$ is entered once. </p><p>In the fourth example, the robot moves as follows: $3 \rightarrow 2 \rightarrow 3 \rightarrow 4 \rightarrow 3 \rightarrow 2$. The robot has completed all instructions from the sequence and is not at $0$. So it stops after $5$ seconds, without reaching the point $0$.</p>
