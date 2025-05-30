## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p><span class="tex-font-style-bf">This is an easy version of the problem. The difference from the hard version is that in the easy version $t=1$ and the number of queries is limited to $20$.</span></p><p>Polycarp is playing a computer game. In this game, an array consisting of zeros and ones is hidden. Polycarp wins if he guesses the position of the $k$-th zero from the left $t$ times.</p><p>Polycarp can make no more than $20$ requests of the following type: </p><ul> <li> <span class="tex-font-style-tt">?</span> $l$ $r$&nbsp;�� find out the sum of all elements in positions from $l$ to $r$ ($1 \le l \le r \le n$) inclusive. </li></ul><p><span class="tex-font-style-it">In this (easy version) of the problem, this paragraph doesn't really make sense since $t=1$ always.</span> To make the game more interesting, each guessed zero turns into one and the game continues on the changed array. More formally, if the position of the $k$-th zero was $x$, then after Polycarp guesses this position, the $x$-th element of the array will be replaced from $0$ to $1$. Of course, this feature affects something only for $t&gt;1$.</p><p>Help Polycarp win the game.</p></div><div><h2>Interaction</h2><p>First, your program must read two integers $n$ and $t$ ($1 \le n \le 2 \cdot 10^5$, $t=1$).</p><p>Then $t$ lines follow, each of which contains one integer $k$ ($1 \le k \le n$). It is guaranteed that at the moment of the request the array contains at least $k$ zeros. In order to get the next value of $k$, you must output the answer for the current value of $k$.</p><p>After that, you can make no more than $20$ requests.</p><p>Use the following format to output the answer (it is not a request, it doesn't count in $20$): </p><ul> <li> <span class="tex-font-style-tt">!</span> $x$&nbsp;�� position of the $k$-th zero. </li></ul><p>Positions in the array are numbered from left to right from $1$ to $n$ inclusive.</p><p>After printing $t$ answers, your program should exit immediately.</p><p>In this task, the interactor is <span class="tex-font-style-bf">not adaptive</span>. This means that within the same test, the hidden array and the queries <span class="tex-font-style-bf">do not change</span>.</p><p>In case of an incorrect query, <span class="tex-font-style-tt">-1</span> will be displayed. When this value is received, your program must immediately exit normally (for example, by calling <span class="tex-font-style-tt">exit(0)</span>), otherwise, the testing system may issue an arbitrary verdict.</p><p>If the number of requests is exceeded, the verdict <span class="tex-font-style-it">wrong answer</span> will be displayed.</p><p>Your solution may get the verdict <span class="tex-font-style-it">Idleness limit exceeded</span> if you don't print anything or forget to flush the output buffer.</p><p>To flush the output buffer, you need to do the following immediately after the query output and the end-of-line character:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C ++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>Use the following format for hacks:</p><p>On the first line print the string $s$ ($1 \le |s| \le 2 \cdot 10^5$), consisting of zeros and ones, and an integer $t$ ($t = 1$)&nbsp;�� hidden array and number of requests, respectively. In the next $t$ lines output the number $k$ ($1 \le k \le |s|$).</p><p>The hacked solution will not have direct access to the hidden array.</p></div>

## Samples

```input1
6 1
2

2

1

1

0

0
```

```output1
? 4 6

? 1 1

? 1 2

? 2 2

? 5 5

! 5
```




## Note

<p>In the first test, the $[1, 0, 1, 1, 0, 1]$ array is hidden. In this test $k=2$.</p>
