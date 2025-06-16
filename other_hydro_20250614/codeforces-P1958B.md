## Description

<div><p>You are swimming in the pool, and you need to control the time of swimming.</p><p>The pool has a clock that cycles between three different modes: showing water temperature, showing air temperature, and showing time. At the start of the $0$-th second it starts showing water temperature, at the start of the $k$-th second it switches to air temperature. At the start of the $2k$-th second, it switches to showing time.</p><p>At the start of the $3k$-th second the clock starts showing water temperature again, at the start of the $4k$-th second&nbsp;�� air temperature, and so on.</p><p>You looked at the clock during the $m$-th second to check the time, but it may be that the clock is not showing time right now. How much time do you have to wait to see the time on the clock?</p><p>Answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases. Next $t$ cases follow.</p><p>The first and only line of each test case contains two integers $k$ and $m$ ($1 \le k \le 10^8; 1 \le m \le 10^9$)&nbsp;�� the length of the period of the clock and the moment of time you check the clock.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;�� the time you have to wait from the moment $m$ until the moment the clock starts showing the time.</p><p>You can assume that you are able to read the time instantly the moment it displays on the clock.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases. Next $t$ cases follow.</p><p>The first and only line of each test case contains two integers $k$ and $m$ ($1 \le k \le 10^8; 1 \le m \le 10^9$)&nbsp;�� the length of the period of the clock and the moment of time you check the clock.</p>

## Output

<p>For each test case, print a single integer&nbsp;�� the time you have to wait from the moment $m$ until the moment the clock starts showing the time.</p><p>You can assume that you are able to read the time instantly the moment it displays on the clock.</p>





```input1|2,4,6
5
1 1
5 14
5 15
10 110
99999999 1000000000
```




```output1
1
0
10
0
99999989
```



## Note

<p>In the first test case, the clock will start showing time during the $2$-nd second, so you have to wait $2 - 1 = 1$ second.</p><p>In the second test case, the clock shows time from the $10$-th until the $15$-th second, so during the $14$-th second it shows time, and you don't have to wait.</p><p>In the third test case, during the $15$-th second, the clock is already showing water temperature. So you have to wait till the $25$-th second, when the clock starts showing time again. You'll wait $25 - 15 = 10$ seconds.</p><p>In the fourth test case, the clock will start showing time at the start of the $110$-th second, so you'll wait $110 - 110 = 0$ seconds.</p>
