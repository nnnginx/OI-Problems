## Description

<div><p>As a computer science student, Alex faces a hard challenge&nbsp;！ showering. He tries to shower daily, but despite his best efforts there are always challenges. He takes $s$ minutes to shower and a day only has $m$ minutes! </p><p>He already has $n$ tasks planned for the day. Task $i$ is represented as an interval $(l_i$, $r_i)$, which means that Alex is busy and can not take a shower in that time interval (at any point in time strictly between $l_i$ and $r_i$). <span class="tex-font-style-bf">No two tasks overlap.</span></p><p>Given all $n$ time intervals, will Alex be able to shower that day? In other words, will Alex have a free time interval of length at least $s$?</p><center> <img class="tex-graphics" src="./34848/file/zF0EtOz5.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">In the first test case, Alex can shower for the first $3$ minutes of the day and not miss any of the tasks.</span> </p></center></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $s$, and $m$ ($1 \leq n \leq 2 \cdot 10^5$; $1 \leq s, m \leq 10^9$)&nbsp;！ the number of time intervals Alex already has planned, the amount of time Alex takes to take a shower, and the amount of minutes a day has.</p><p>Then $n$ lines follow, the $i$-th of which contains two integers $l_i$ and $r_i$ ($0 \leq l_i &lt; r_i \leq m$)&nbsp;！ the time interval of the $i$-th task. No two tasks overlap.</p><p><span class="tex-font-style-bf">Additional constraint on the input:</span> $l_i &gt; r_{i-1}$ for every $i &gt; 1$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alex can take a shower for that given test case, and "<span class="tex-font-style-tt">NO</span>" (also without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $s$, and $m$ ($1 \leq n \leq 2 \cdot 10^5$; $1 \leq s, m \leq 10^9$)&nbsp;！ the number of time intervals Alex already has planned, the amount of time Alex takes to take a shower, and the amount of minutes a day has.</p><p>Then $n$ lines follow, the $i$-th of which contains two integers $l_i$ and $r_i$ ($0 \leq l_i &lt; r_i \leq m$)&nbsp;！ the time interval of the $i$-th task. No two tasks overlap.</p><p><span class="tex-font-style-bf">Additional constraint on the input:</span> $l_i &gt; r_{i-1}$ for every $i &gt; 1$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alex can take a shower for that given test case, and "<span class="tex-font-style-tt">NO</span>" (also without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,4,5,10,11,12,13
4
3 3 10
3 5
6 8
9 10
3 3 10
1 2
3 5
6 7
3 3 10
1 2
3 5
6 8
3 4 10
1 2
6 7
8 9
```




```output1
YES
YES
NO
YES
```


