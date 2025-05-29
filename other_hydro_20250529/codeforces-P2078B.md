## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/1HyuI8Bvnsg?si=6amlU5OPKnJiydZs"><span class="tex-font-style-it">Axium Crisis - ak+q</span></a></div><div class="epigraph-source"> </div></div><p>There are $n$ cells in a labyrinth, and cell $i$ ($1 \leq i \leq n$) is $n - i$ kilometers away from the exit. In particular, cell $n$ is the exit. Note also that each cell is connected to the exit but is not accessible from any other cell in any way.</p><p>In each cell, there is initially exactly one person stuck in it. You want to help everyone get as close to the exit as possible by installing a teleporter in each cell $i$ ($1 \leq i \leq n$), which translocates the person in that cell to another cell $a_i$.</p><p>The labyrinth owner caught you in the act. Amused, she let you continue, but under some conditions:</p><ul><li> Everyone must use the teleporter exactly $k$ times.</li><li> No teleporter in any cell can lead to the same cell it is in. Formally, $i \neq a_i$ for all $1 \leq i \leq n$.</li></ul><p>You must find a teleporter configuration that minimizes the sum of distances of all individuals from the exit after using the teleporter exactly $k$ times while still satisfying the restrictions of the labyrinth owner.</p><p>If there are many possible configurations, you can output any of them.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains two integers $n$ and $k$ ($2 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 10^9$)&nbsp;！ the number of cells in the labyrinth and the value $k$.</p><p>It is guaranteed that the total sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers&nbsp;！ the destinations of the teleporters $a_1, a_2, \ldots, a_n$ in order, satisfying the given conditions ($1 \leq a_i \leq n$, $a_i \neq i$).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains two integers $n$ and $k$ ($2 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 10^9$)&nbsp;！ the number of cells in the labyrinth and the value $k$.</p><p>It is guaranteed that the total sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers&nbsp;！ the destinations of the teleporters $a_1, a_2, \ldots, a_n$ in order, satisfying the given conditions ($1 \leq a_i \leq n$, $a_i \neq i$).</p>





```input1|2
2
2 1
3 2
```




```output1
2 1
2 3 2
```



## Note

<p>In the first test case, the position of each person is as follows.</p><ul><li> Before teleporting: $[1, 2]$.</li><li> First teleportation: $[2, 1]$.</li></ul><p>The distance sum is $(2-2) + (2-1) = 1$, which is the minimum possible.</p><p>In the second test case, the position of each person is as follows.</p><ul><li> Before teleporting: $[1, 2, 3]$.</li><li> First teleportation: $[2, 3, 2]$.</li><li> Second teleportation: $[3, 2, 3]$.</li></ul><p>The distance sum is $(3-3) + (3-2) + (3-3) = 1$, which is the minimum possible.</p>
