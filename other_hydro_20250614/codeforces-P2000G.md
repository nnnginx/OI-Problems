## Description

<div><p>You live in a city consisting of $n$ intersections and $m$ streets connecting some pairs of intersections. You can travel in either direction on each street. No two streets connect the same pair of intersections, and no street connects an intersection to itself. You can reach any intersection from any other, possibly passing through some other intersections.</p><p>Every minute, you can board a bus at intersection $u_i$ and travel for $l_{i1}$ minutes to intersection $v_i$. Conversely, you can travel from intersection $v_i$ to intersection $u_i$ in $l_{i1}$ minutes. You can only board and exit the bus at intersections. You can only board the bus at an intersection if you are currently there.</p><p>You can also walk along each street, which takes $l_{i2} &gt; l_{i1}$ minutes.</p><p>You can make stops at intersections.</p><p>You live at intersection number $1$. Today you woke up at time $0$, and you have an important event scheduled at intersection number $n$, which you must reach no later than time $t_0$. You also have a phone call planned that will last from $t_1$ to $t_2$ minutes ($t_1 &lt; t_2 &lt; t_0$). </p><p>During the phone call, you cannot ride the bus, but you can walk along any streets, make stops, or stay at home. You can exit the bus at minute $t_1$ and board the bus again at minute $t_2$.</p><p>Since you want to get enough sleep, you became curious �� how late can you leave home to have time to talk on the phone and still not be late for the event?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) �� the number of test cases. The following are the descriptions of the test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 10^5, 1 \le m \le 10^5$) �� the number of intersections and streets in the city.</p><p>The second line of each test case contains three integers $t_0$, $t_1$, $t_2$ ($1 \le t_1 &lt; t_2 &lt; t_0 \le 10^9$) �� the start time of the event, the start time of the phone call, and its end time, respectively.</p><p>The next $m$ lines of each test case contain descriptions of the streets.</p><p>The $i$-th line contains four integers $u_i$, $v_i$, $l_{i1}$, $l_{i2}$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$, $1 \le l_{i1} &lt; l_{i2} \le 10^9$) �� the numbers of the intersections connected by the $i$-th street, as well as the travel time along the street by bus and on foot. It is guaranteed that no two streets connect the same pair of intersections and that it is possible to reach any intersection from any other.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $10^5$. It is also guaranteed that the sum of the values of $m$ across all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the latest time you can leave home to have time to talk on the phone and not be late for the event. If you cannot reach the event on time, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) �� the number of test cases. The following are the descriptions of the test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 10^5, 1 \le m \le 10^5$) �� the number of intersections and streets in the city.</p><p>The second line of each test case contains three integers $t_0$, $t_1$, $t_2$ ($1 \le t_1 &lt; t_2 &lt; t_0 \le 10^9$) �� the start time of the event, the start time of the phone call, and its end time, respectively.</p><p>The next $m$ lines of each test case contain descriptions of the streets.</p><p>The $i$-th line contains four integers $u_i$, $v_i$, $l_{i1}$, $l_{i2}$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$, $1 \le l_{i1} &lt; l_{i2} \le 10^9$) �� the numbers of the intersections connected by the $i$-th street, as well as the travel time along the street by bus and on foot. It is guaranteed that no two streets connect the same pair of intersections and that it is possible to reach any intersection from any other.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $10^5$. It is also guaranteed that the sum of the values of $m$ across all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer �� the latest time you can leave home to have time to talk on the phone and not be late for the event. If you cannot reach the event on time, output <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,3,4,5,6,7,8,12,13,14,15,16,17,23,24,25,26,30,31,32,33,34,35,36
7
5 5
100 20 80
1 5 30 100
1 2 20 50
2 3 20 50
3 4 20 50
4 5 20 50
2 1
100 50 60
1 2 55 110
4 4
100 40 60
1 2 30 100
2 4 30 100
1 3 20 50
3 4 20 50
3 3
100 80 90
1 2 1 10
2 3 10 50
1 3 20 21
3 2
58 55 57
2 1 1 3
2 3 3 4
2 1
12 9 10
2 1 6 10
5 5
8 5 6
2 1 1 8
2 3 4 8
4 2 2 4
5 3 3 4
4 5 2 6
```




```output1
0
-1
60
80
53
3
2
```


