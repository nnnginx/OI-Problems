## Description

<div><p>The snails are climbing a tree. The tree height is $h$ meters, and snails start at position $0$.</p><p>Each snail has two attributes $a$ and $b$ ($a &gt; b$). Starting from the $1$-st day, one snail climbs the tree like this: during the daylight hours of the day, he climbs up $a$ meters; during the night, the snail rests, and he slides down $b$ meters. If on the $n$-th day, the snail reaches position $h$ for the first time (that is, the top of the tree), he will finish climbing, and we say that the snail spends $n$ days climbing the tree. Note that on the last day of climbing, the snail doesn't necessarily climb up $a$ meters, in case his distance to the top is smaller than $a$.</p><p>Unfortunately, you don't know the exact tree height $h$ at first, but you know that $h$ is a positive integer. There are $q$ events of two kinds.</p><ul> <li> Event of type $1$: a snail with attributes $a$, $b$ comes and claims that he spent $n$ days climbing the tree. If this message contradicts previously adopted information (i.&nbsp;e. there is no tree for which all previously adopted statements and this one are true), ignore it. Otherwise, adopt it.</li><li> Event of type $2$: a snail with attributes $a$, $b$ comes and asks you how many days he will spend if he climbs the tree. You can only give the answer based on the information you have adopted so far. If you cannot determine the answer precisely, report that. </li></ul><p>You need to deal with all the events in order.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$) �� the number of test cases. Then follows their description.</p><p>The first line of each test case contains one integer $q$ ($1\le q \le 2\cdot 10^5$) �� the number of events.</p><p>For the following $q$ lines, the first integer of each line is either $1$ or $2$, denoting the event type.</p><p>If the event type is $1$, then three integers $a$, $b$, and $n$ ($1\le a,b,n \le 10^9$, $a&gt;b$) follow.</p><p>If the event type is $2$, then two integers $a$ and $b$ ($1\le a,b \le 10^9$, $a&gt;b$) follow.</p><p>It is guaranteed that the sum of $q$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $q$ integers in one line, one for each event, in order. Specifically, </p><ul> <li> for each event of type $1$, if you adopt the message, output $1$; if you ignore it, output $0$; </li><li> for each event of type $2$, output an integer denoting the number of days that the snail will spend. If you cannot determine it, output $-1$. </li></ul></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$) �� the number of test cases. Then follows their description.</p><p>The first line of each test case contains one integer $q$ ($1\le q \le 2\cdot 10^5$) �� the number of events.</p><p>For the following $q$ lines, the first integer of each line is either $1$ or $2$, denoting the event type.</p><p>If the event type is $1$, then three integers $a$, $b$, and $n$ ($1\le a,b,n \le 10^9$, $a&gt;b$) follow.</p><p>If the event type is $2$, then two integers $a$ and $b$ ($1\le a,b \le 10^9$, $a&gt;b$) follow.</p><p>It is guaranteed that the sum of $q$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $q$ integers in one line, one for each event, in order. Specifically, </p><ul> <li> for each event of type $1$, if you adopt the message, output $1$; if you ignore it, output $0$; </li><li> for each event of type $2$, output an integer denoting the number of days that the snail will spend. If you cannot determine it, output $-1$. </li></ul>





```input1|2,3,4,5,10,11,12,13,24,25,26,27,28,29,30,31,32,33
5
3
1 3 2 5
2 4 1
2 3 2
3
1 6 5 1
2 3 1
2 6 2
3
1 4 2 2
1 2 1 3
2 10 2
9
1 7 3 6
1 2 1 8
2 5 1
1 10 9 7
1 8 1 2
1 10 5 8
1 10 7 7
2 7 4
1 9 4 2
9
1 2 1 6
1 8 5 6
1 4 2 7
2 9 1
1 5 1 4
1 5 2 7
1 7 1 9
1 9 1 4
2 10 8
```




```output1
1 2 5
1 -1 1
1 0 1
1 0 -1 0 0 0 1 8 0
1 0 0 1 0 0 0 0 1
```



## Note

<p>In the first test case, we can determine $h=7$ through the first message, so we know the second snail and the third snail need to spend $2$ and $5$ days respectively to reach the top.</p><p>Let's show how the second snail climbs:</p><ul> <li> During the daylight hours of the $1$st day: climbs up $4$ meters, now at position $4$. </li><li> During the night of the $1$st day: slides down $1$ meters, now at position $3$. </li><li> During the daylight hours of the $2$nd day: climbs up $4$ meters, now at position $7$ (reaches the top). </li></ul><p>In the third test case, the second snail's message contradicts the first snail's, because the second snail says he spent $3$ days, and he can climb at most $1+1+2=4$ meters in the first $3$ days. However, the first snail only needs $1$ day to climb $4$ meters.</p>
