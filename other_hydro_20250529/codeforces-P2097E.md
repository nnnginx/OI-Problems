## Description

<div><p>Boy Vasya loves to travel very much. In particular, flying in airplanes brings him extraordinary pleasure. He was about to fly to another city, but the runway was heavily covered with snow and needed to be cleared.</p><p>The runway can be represented as $n$ consecutive sections numbered from $1$ to $n$. The snowstorm was quite strong, but it has already stopped, so Vasya managed to calculate that the $i$-th section is covered with $a_i$ meters of snow. For such situations, the airport has a snowplow that works in a rather unusual way. In one minute, the snowplow can do the following:</p><ul> <li> Choose a consecutive segment of length no more than $d$ and remove one meter of snow from the most snow-covered sections.<p>Formally, one can choose $1 \le l \le r \le n$ ($r - l + 1 \le d$). After that, $c = \max \{ a_l, a_{l + 1}, \ldots , a_r \}$ is calculated, and if $c &gt; 0$, then for all $i \colon l \le i \le r$ such that $a_i = c$, the value of $a_i$ is decreased by one. </p></li></ul><p>Vasya has been preparing for the flight for a long time and wants to understand how much time he has left to wait until all sections are completely cleared of snow. In other words, it is required to calculate the minimum number of minutes that the snowplow will need to achieve $a_i = 0$ for all $i$ from $1$ to $n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $d$ ($1 \le n \le 5 \cdot 10^5, 1 \le d \le n$) �� the number of sections on the runway and the maximum length of the segment that the snowplow can choose.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of meters of snow on the $i$-th section.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;�� the minimum number of minutes required for the snowplow to achieve $a_i = 0$ for all $i$ from $1$ to $n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $d$ ($1 \le n \le 5 \cdot 10^5, 1 \le d \le n$) �� the number of sections on the runway and the maximum length of the segment that the snowplow can choose.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of meters of snow on the $i$-th section.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;�� the minimum number of minutes required for the snowplow to achieve $a_i = 0$ for all $i$ from $1$ to $n$.</p>





```input1|2,3
2
5 2
1 5 2 1 2
3 1
1000000000 1000000000 1000000000
```




```output1
8
3000000000
```



## Note

<p>In the first test case, there is an optimal sequence of operations. First, select the segment $[2, 3]$ four times. After three operations, $a_2$ will turn into $2$, and the array $a$ will look like $[1, 2, 2, 1, 2]$. After the fourth operation, the array $a$ will become $[1, 1, 1, 1, 2]$. Next, the array can be transformed into zeros by selecting the segments $[1, 2]$, $[3, 3]$, $[5, 5]$, and $[4, 5]$ (in that exact order).</p><p>In the second test case, $d = 1$, which means that each section is cleared independently of the others, and the answer is equal to the sum of all $a_i$.</p>
