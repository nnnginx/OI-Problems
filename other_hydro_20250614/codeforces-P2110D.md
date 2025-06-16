## Description

<div><p>In 2077, when robots took over the world, they decided to compete in the following game.</p><p>There are $n$ checkpoints, and the $i$-th checkpoint contains $b_i$ batteries. Initially, the Robot starts at the $1$-st checkpoint with no batteries and must reach the $n$-th checkpoint.</p><p>There are a total of $m$ one-way passages between the checkpoints. The $i$-th passage allows movement from point $s_i$ to point $t_i$ ($s_i &lt; t_i$), but not the other way. Additionally, the $i$-th passage can only be used if the robot has at least $w_i$ charged batteries; otherwise, it will run out of power on the way.</p><p>When the robot arrives at point $v$, it can additionally take any number of batteries from $0$ to $b_v$, inclusive. Moreover, it always carries all previously collected batteries, and at each checkpoint, it recharges all previously collected batteries.</p><p>Find the minimum number of batteries that the robot can have at the end of the journey, or report that it is impossible to reach from the first checkpoint to the last.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n, m$ ($2 \leq n \leq 2 \cdot 10^5, 0 \leq m \leq 3 \cdot 10^5$)&nbsp;！ the number of checkpoints and the number of passages, respectively.</p><p>The second line contains $n$ numbers $b_i$ ($0 \leq b_i \leq 10^9$)&nbsp;！ the number of batteries at the $i$-th checkpoint.</p><p>The next $m$ lines contain three integers $s_i, t_i, w_i$ ($1 \leq s_i &lt; t_i \leq n, 1 \leq w_i \leq 10^9$)&nbsp;！ the endpoints of the passage and the minimum number of batteries required to pass through it.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of $m$ does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the minimum number of batteries that you can have at the end of the journey, or $-1$ if it is impossible to reach point $n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n, m$ ($2 \leq n \leq 2 \cdot 10^5, 0 \leq m \leq 3 \cdot 10^5$)&nbsp;！ the number of checkpoints and the number of passages, respectively.</p><p>The second line contains $n$ numbers $b_i$ ($0 \leq b_i \leq 10^9$)&nbsp;！ the number of batteries at the $i$-th checkpoint.</p><p>The next $m$ lines contain three integers $s_i, t_i, w_i$ ($1 \leq s_i &lt; t_i \leq n, 1 \leq w_i \leq 10^9$)&nbsp;！ the endpoints of the passage and the minimum number of batteries required to pass through it.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of $m$ does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output the minimum number of batteries that you can have at the end of the journey, or $-1$ if it is impossible to reach point $n$.</p>





```input1|2,3,4,5,6,15,16
4
3 3
2 0 0
1 2 1
2 3 1
1 3 2
5 6
2 2 5 0 1
1 2 2
1 3 1
1 4 3
3 5 5
2 4 4
4 5 3
2 0
1 1
4 4
3 10 0 0
1 2 1
1 3 3
2 3 10
3 4 5
```




```output1
1
4
-1
10
```



## Note

<p>In the first test case, you need to take $1$ battery at the starting point, then move to point $2$, and then to point $3$.</p><p>In the second test case, you need to take $2$ batteries at the starting point, then move to point $2$, take another $2$ batteries, move to point $4$, and then to point $5$.</p><p>In the third test case, there is no path from point $1$ to point $n$.</p><p>In the fourth test case, you need to take $1$ battery at the starting point, then move to point $2$, take another $9$ batteries, move to point $3$, and then to point $4$. </p>
