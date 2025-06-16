## Description

<div><p>Turtle and Piggy are playing a game on a sequence. They are given a sequence $a_1, a_2, \ldots, a_n$, and Turtle goes first. Turtle and Piggy alternate in turns (so, Turtle does the first turn, Piggy does the second, Turtle does the third, etc.).</p><p>The game goes as follows:</p><ul> <li> Let the current length of the sequence be $m$. If $m = 1$, the game ends. </li><li> If the game does not end and it's Turtle's turn, then Turtle must choose an integer $i$ such that $1 \le i \le m - 1$, set $a_i$ to $\max(a_i, a_{i + 1})$, and remove $a_{i + 1}$. </li><li> If the game does not end and it's Piggy's turn, then Piggy must choose an integer $i$ such that $1 \le i \le m - 1$, set $a_i$ to $\min(a_i, a_{i + 1})$, and remove $a_{i + 1}$. </li></ul><p>Turtle wants to <span class="tex-font-style-bf">maximize</span> the value of $a_1$ in the end, while Piggy wants to <span class="tex-font-style-bf">minimize</span> the value of $a_1$ in the end. Find the value of $a_1$ in the end if both players play optimally.</p><p>You can refer to notes for further clarification.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) �� the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$) �� the elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the value of $a_1$ in the end if both players play optimally.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) �� the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$) �� the elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer �� the value of $a_1$ in the end if both players play optimally.</p>





```input1|2,3,6,7,10,11
5
2
1 2
3
1 1 2
3
1 2 3
5
3 1 2 2 3
10
10 2 5 2 7 9 2 5 10 7
```




```output1
2
1
2
2
7
```



## Note

<p>In the first test case, initially $a = [1, 2]$. Turtle can only choose $i = 1$. Then he will set $a_1$ to $\max(a_1, a_2) = 2$ and remove $a_2$. The sequence $a$ becomes $[2]$. Then the length of the sequence becomes $1$, and the game will end. The value of $a_1$ is $2$, so you should output $2$.</p><p>In the second test case, one of the possible game processes is as follows:</p><ul> <li> Initially $a = [1, 1, 2]$. </li><li> Turtle can choose $i = 2$. Then he will set $a_2$ to $\max(a_2, a_3) = 2$ and remove $a_3$. The sequence $a$ will become $[1, 2]$. </li><li> Piggy can choose $i = 1$. Then he will set $a_1$ to $\min(a_1, a_2) = 1$ and remove $a_2$. The sequence $a$ will become $[1]$. </li><li> The length of the sequence becomes $1$, so the game will end. The value of $a_1$ will be $1$ in the end. </li></ul><p>In the fourth test case, one of the possible game processes is as follows:</p><ul> <li> Initially $a = [3, 1, 2, 2, 3]$. </li><li> Turtle can choose $i = 4$. Then he will set $a_4$ to $\max(a_4, a_5) = 3$ and remove $a_5$. The sequence $a$ will become $[3, 1, 2, 3]$. </li><li> Piggy can choose $i = 3$. Then he will set $a_3$ to $\min(a_3, a_4) = 2$ and remove $a_4$. The sequence $a$ will become $[3, 1, 2]$. </li><li> Turtle can choose $i = 2$. Then he will set $a_2$ to $\max(a_2, a_3) = 2$ and remove $a_3$. The sequence $a$ will become $[3, 2]$. </li><li> Piggy can choose $i = 1$. Then he will set $a_1$ to $\min(a_1, a_2) = 2$ and remove $a_2$. The sequence $a$ will become $[2]$. </li><li> The length of the sequence becomes $1$, so the game will end. The value of $a_1$ will be $2$ in the end. </li></ul>
