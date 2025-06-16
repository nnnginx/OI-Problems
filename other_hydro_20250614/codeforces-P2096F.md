## Description

<div><p>You are a proud live streamer known as Gigi Murin. Today, you will play a game with $n$ viewers numbered $1$ to $n$.</p><p>In the game, each player is either a crewmate or an impostor. You don't know the role of each viewer.</p><p>There are $m$ statements numbered $1$ to $m$, which are either <span class="tex-font-style-bf">true or false</span>. For each $i$ from $1$ to $m$, statement $i$ is one of two types:</p><ul><li> $0\:a_i\:b_i$ ($1 \leq a_i \leq b_i \leq n$)&nbsp;！ there are no impostors among viewers $a_i, a_i + 1, \ldots, b_i$;</li><li> $1\:a_i\:b_i$ ($1 \leq a_i \leq b_i \leq n$)&nbsp;！ there is <span class="tex-font-style-bf">at least</span> one impostor among viewers $a_i, a_i + 1, \ldots, b_i$.</li></ul><p>Answer $q$ questions of the following form:</p><ul><li> $l\:r$ ($1 \leq l \leq r \leq m$)&nbsp;！ is it possible that statements $l, l + 1, \ldots, r$ are <span class="tex-font-style-bf">all true</span>?</li></ul><p>Note that it is <span class="tex-font-style-bf">not guaranteed</span> that there is at least one impostor among all viewers, and it is <span class="tex-font-style-bf">not guaranteed</span> that there is at least one crewmate among all viewers.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n, m \leq 2 \cdot 10^5$)&nbsp;！ the number of viewers, and the number of statements.</p><p>The $i$-th of the next $m$ lines contains three integers $x_i$, $a_i$, $b_i$ ($x_i \in \{0, 1\}$, $1 \leq a_i \leq b_i \leq n$)&nbsp;！ describing statement $i$.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of questions.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \leq l \leq r \leq m$)&nbsp;！ describing a question.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$, the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each question, output "<span class="tex-font-style-tt">YES</span>" if it is possible that the requested statements are all true. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n, m \leq 2 \cdot 10^5$)&nbsp;！ the number of viewers, and the number of statements.</p><p>The $i$-th of the next $m$ lines contains three integers $x_i$, $a_i$, $b_i$ ($x_i \in \{0, 1\}$, $1 \leq a_i \leq b_i \leq n$)&nbsp;！ describing statement $i$.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of questions.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \leq l \leq r \leq m$)&nbsp;！ describing a question.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$, the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each question, output "<span class="tex-font-style-tt">YES</span>" if it is possible that the requested statements are all true. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,5,6,7,15,16,17,18,19,20
4
4 3
1 1 3
1 2 4
0 2 3
1
1 3
5 2
0 1 5
1 1 5
3
1 1
2 2
1 2
1 2
0 1 1
1 1 1
2
1 1
2 2
7 9
1 2 2
1 4 5
0 5 6
1 2 2
1 1 1
0 4 7
0 3 7
0 2 7
0 6 6
5
1 5
2 6
3 7
4 8
5 9
```




```output1
YES
YES
YES
NO
YES
YES
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, there are $4$ viewers and $3$ statements. The statements are as follows:</p><ul> <li> Statement $1$: There is at least one impostor among viewers $1$, $2$, and $3$; </li><li> Statement $2$: There is at least one impostor among viewers $2$, $3$, and $4$; </li><li> Statement $3$: There are no impostors among viewers $2$ and $3$. </li></ul><p>We can see that it is possible that statements $1$, $2$, and $3$ are all true. For example, this is one possible scenario:</p><ul> <li> Viewer $1$ is an impostor; </li><li> Viewer $2$ is a crewmate; </li><li> Viewer $3$ is a crewmate; </li><li> Viewer $4$ is an impostor. </li></ul><p>In the second test case, there are $5$ viewers and $2$ statements. The statements are as follows:</p><ul> <li> Statement $1$: There is at least one impostor among viewers $1$, $2$, $3$, $4$, and $5$; </li><li> Statement $2$: There are no impostors among viewers $1$, $2$, $3$, $4$, and $5$. </li></ul><p>We can see that it is possible that statement $1$ is true, and it is possible that statement $2$ is true. However, it is not possible that both statements $1$ and $2$ are true.</p>
