## Description

<div><p>Vanya has a graph with $n$ vertices (numbered from $1$ to $n$) and an array $a$ of $n$ integers; initially, there are no edges in the graph. Vanya got bored, and to have fun, he decided to perform $n - 1$ operations.</p><p>Operation number $x$ (operations are numbered in order starting from $1$) is as follows:</p><ul> <li> Choose $2$ different numbers $1 \leq u,v \leq n$, such that $|a_u - a_v|$ is divisible by $x$. </li><li> Add an undirected edge between vertices $u$ and $v$ to the graph. </li></ul><p>Help Vanya get a connected$^{\text{∗}}$ graph using the $n - 1$ operations, or determine that it is impossible.</p><div class="statement-footnote"><p>$^{\text{∗}}$A graph is called connected if it is possible to reach any vertex from any other by moving along the edges.</p></div></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{3}$)&nbsp;— the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains the number $n$ ($1 \leq n \leq 2000$)&nbsp;— the number of vertices in the graph.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \cdots a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, if there is no solution, then output "<span class="tex-font-style-tt">No</span>" (without quotes). </p><p>Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes), and then output $n - 1$ lines, where in the $i$-th line, output the numbers $u$ and $v$ that need to be chosen for operation $i$.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{3}$)&nbsp;— the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains the number $n$ ($1 \leq n \leq 2000$)&nbsp;— the number of vertices in the graph.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \cdots a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, if there is no solution, then output "<span class="tex-font-style-tt">No</span>" (without quotes). </p><p>Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes), and then output $n - 1$ lines, where in the $i$-th line, output the numbers $u$ and $v$ that need to be chosen for operation $i$.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11,14,15
8
2
1 4
4
99 7 1 13
5
10 2 31 44 73
5
87 6 81 44 32
5
62 35 33 79 16
5
6 51 31 69 42
5
52 63 25 21 5
12
33 40 3 11 31 43 37 8 50 5 12 22
```




```output1
YES
2 1
YES
4 1
2 1
3 2
YES
5 1
4 1
3 1
2 1
YES
4 1
3 1
2 1
5 4
YES
3 1
5 1
2 1
4 2
YES
4 1
5 1
2 1
3 2
YES
2 1
5 2
3 1
4 3
YES
9 1
12 9
11 1
10 1
6 1
7 6
2 1
8 2
5 2
3 1
4 1
```



## Note

<p>Let's consider the second test case. </p><ul> <li> First operation $(x = 1)$: we can connect vertices $4$ and $1$, since $|a_4 - a_1| = |13 - 99| = |-86| = 86$, and $86$ is divisible by $1$. </li></ul> <img class="tex-graphics" src="./34815/file/8bWGHI8p.png" style="max-width: 100.0%;max-height: 100.0%;"> <ul> <li> Second operation $(x = 2)$: we can connect vertices $2$ and $1$, since $|a_2 - a_1| = |7 - 99| = |-92| = 92$, and $92$ is divisible by $2$. </li></ul> <img class="tex-graphics" src="./34815/file/N2gYOWkH.png" style="max-width: 100.0%;max-height: 100.0%;"> <ul> <li> Third operation $(x = 3)$: we can connect vertices $3$ and $2$, since $|a_3 - a_2| = |1 - 7| = |-6| = 6$, and $6$ is divisible by $3$. </li></ul> <img class="tex-graphics" src="./34815/file/3YiHyoRb.png" style="max-width: 100.0%;max-height: 100.0%;"> From the picture, it can be seen that a connected graph is obtained.
