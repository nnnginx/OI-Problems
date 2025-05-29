## Description

<div><p>Define the <span class="tex-font-style-it">range</span> of a non-empty array to be the maximum value minus the minimum value. For example, the range of $[1,4,2]$ is $4-1=3$.</p><p>You are given an array $a_1, a_2, \ldots, a_n$ of length $n \geq 3$. <span class="tex-font-style-bf">It is guaranteed $a$ is sorted</span>.</p><p>You have to color each element of $a$ red or blue so that: </p><ul> <li> the range of the red elements <span class="tex-font-style-bf">does not equal</span> the range of the blue elements, and </li><li> there is at least one element of each color. </li></ul><p><span class="tex-font-style-bf">If there does not exist any such coloring, you should report it.</span> If there are multiple valid colorings, you can print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 50$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$). It is guaranteed $a_1 \leq a_2 \leq \ldots \leq a_{n - 1} \leq a_{n}$.</p></div><div class="output-specification"><p>For each test case, if it is impossible to color $a$ to satisfy all the constraints, output $\texttt{NO}$.</p><p>Otherwise, first output $\texttt{YES}$.</p><p>Then, output a string $s$ of length $n$. For $1 \leq i \leq n$, if you color $a_i$ red, $s_i$ should be $\texttt{R}$. For $1 \leq i \leq n$, if you color $a_i$ blue, $s_i$ should be $\texttt{B}$. </p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 50$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$). It is guaranteed $a_1 \leq a_2 \leq \ldots \leq a_{n - 1} \leq a_{n}$.</p>

## Output

<p>For each test case, if it is impossible to color $a$ to satisfy all the constraints, output $\texttt{NO}$.</p><p>Otherwise, first output $\texttt{YES}$.</p><p>Then, output a string $s$ of length $n$. For $1 \leq i \leq n$, if you color $a_i$ red, $s_i$ should be $\texttt{R}$. For $1 \leq i \leq n$, if you color $a_i$ blue, $s_i$ should be $\texttt{B}$. </p>





```input1|2,3,6,7,10,11,14,15
7
4
1 1 2 2
5
1 2 3 4 5
3
3 3 3
4
1 2 2 2
3
1 2 2
3
1 1 2
3
1 9 84
```




```output1
YES
RBRR
YES
BBRBB
NO
YES
RBBR
YES
RRB
YES
BRR
YES
BRB
```



## Note

<p>In the first test case, given the array $[1, 1, 2, 2]$, we can color the second element blue and the remaining elements red; then the range of the red elements $[1, 2, 2]$ is $2-1=1$, and the range of the blue elements $[1]$ is $1-1=0$.</p><p>In the second test case, we can color the first, second, fourth and fifth elements $[1, 2, 4, 5]$ blue and the remaining elements $[3]$ red. </p><p>The range of the red elements is $3 - 3 = 0$ and the range of the blue elements is $5 - 1 = 4$, which are different.</p><p>In the third test case, it can be shown there is no way to color $a = [3, 3, 3]$ to satisfy the constraints.</p>
