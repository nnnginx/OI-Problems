## Description

<div><p>Little B and his friend Little K found a treasure map, and now they just need to dig up the treasure, which is buried at a depth of $a.5$ meters.</p><p>They take turns digging. On the first day, Little B digs; on the second day, Little K. After each day, they switch. Little B digs exactly $x$ meters of soil each day, while Little K digs $y$ meters. They became curious about who will dig up the treasure first, meaning during whose day the total dug depth will exceed $a.5$.</p><p>But they are too busy digging, so help them and tell who will dig up the treasure!</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>In a single line of each test case, three integers $x, y, a$ are given ($1 \leq x, y, a \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, output "NO" if Little B digs it up first; otherwise, output "YES". You can output the answer in any case.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>In a single line of each test case, three integers $x, y, a$ are given ($1 \leq x, y, a \leq 10^9$).</p>

## Output

<p>For each test case, output "NO" if Little B digs it up first; otherwise, output "YES". You can output the answer in any case.</p>





```input1|2,4
3
1 2 4
2 1 4
2 2 1
```




```output1
YES
NO
NO
```



## Note

<p>In the first test case, on the first day they will dig $1$ meter; on the second day $1 + 2 = 3$ meters in total; on the third day $1 + 2 + 1 = 4$ meters; and on the fourth day they will dig $6$ meters. Thus, the treasure will be dug up first by Little K.</p><p>In the second test case, on the first day they will dig $2$ meters; on the second day $2 + 1 = 3$ meters in total; on the third day $2 + 1 + 2 = 5$ meters, meaning it was dug up first by Little B.</p>
