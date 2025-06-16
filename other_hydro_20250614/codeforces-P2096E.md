## Description

<div><p>You are the proud owner of $n$ teddy bears, which are arranged in a row on a shelf. Each teddy bear is colored either black or pink.</p><p>An arrangement of teddy bears is <span class="tex-font-style-it">beautiful</span> if all the black teddy bears are to the left of all the pink teddy bears. In other words, there <span class="tex-font-style-bf">does not</span> exist a pair of indices $(i, j)$ ($1 \leq i &lt; j \leq n$) such that the $i$-th teddy bear is pink, and the $j$-th teddy bear is black.</p><p>You want to reorder the teddy bears into a beautiful arrangement. You are too short to reach the shelf, but luckily, you can send instructions to a robot to move the teddy bears around. In a single instruction, the robot can:</p><ul> <li> Choose an index $i$ ($1 \le i \le n - 2$) and reorder the teddy bears at positions $i$, $i + 1$ and $i + 2$ so that all the black teddy bears are to the left of all the pink teddy bears. </li></ul><p>What is the minimum number of instructions needed to reorder the teddy bears?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of teddy bears.</p><p>The second line of each test case contains a single string $s$ of length $n$ consisting of characters <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">P</span>&nbsp;！ the colors of the teddy bears. For each $i$ from $1$ to $n$, the $i$-th teddy bear is colored black if $s_i = \texttt{B}$ and pink if $s_i = \texttt{P}$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of instructions needed to reorder the teddy bears.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of teddy bears.</p><p>The second line of each test case contains a single string $s$ of length $n$ consisting of characters <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">P</span>&nbsp;！ the colors of the teddy bears. For each $i$ from $1$ to $n$, the $i$-th teddy bear is colored black if $s_i = \texttt{B}$ and pink if $s_i = \texttt{P}$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of instructions needed to reorder the teddy bears.</p>





```input1|2,3,6,7,10,11
5
3
PPP
3
BPP
3
PPB
7
PPBPPBB
15
BPBPBBBBBPBBBBB
```




```output1
0
0
1
5
14
```



## Note

<p>For the first test case, all the teddy bears are pink. Thus, the arrangement is already beautiful, so the answer is $0$.</p><p>For the second test case, all the black teddy bears are to the left of all the pink teddy bears. Thus, the answer is $0$.</p><p>For the third test case, we can perform $1$ instruction with $i = 1$.</p><p>After the instruction, the sequence of colors changes from $\texttt{PPB}$ to $\texttt{BPP}$, and we are done.</p><p>For the fourth test case, we can perform $5$ instructions as follows:</p><ul> <li> $i = 1$: $\texttt{}\color{magenta}{\texttt{PPB}}\texttt{PPBB} \rightarrow \texttt{}\color{magenta}{\texttt{BPP}}\texttt{PPBB}$ </li><li> $i = 5$: $\texttt{BPPP}\color{magenta}{\texttt{PBB}}\texttt{} \rightarrow \texttt{BPPP}\color{magenta}{\texttt{BBP}}\texttt{}$ </li><li> $i = 4$: $\texttt{BPP}\color{magenta}{\texttt{PBB}}\texttt{P} \rightarrow \texttt{BPP}\color{magenta}{\texttt{BBP}}\texttt{P}$ </li><li> $i = 3$: $\texttt{BP}\color{magenta}{\texttt{PBB}}\texttt{PP} \rightarrow \texttt{BP}\color{magenta}{\texttt{BBP}}\texttt{PP}$ </li><li> $i = 2$: $\texttt{B}\color{magenta}{\texttt{PBB}}\texttt{PPP} \rightarrow \texttt{B}\color{magenta}{\texttt{BBP}}\texttt{PPP}$ </li></ul>
