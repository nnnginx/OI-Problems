## Description

<div><p> </p><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that in this version, there are no additional limits on $k$. You can hack only if you solved all versions of this problem.</span> </p><p>Ecrade has two sequences $a_0, a_1, \ldots, a_{n - 1}$ and $b_0, b_1, \ldots, b_{n - 1}$ consisting of integers. It is guaranteed that the sum of all elements in $a$ does not exceed the sum of all elements in $b$.</p><p>Initially, Ecrade can make exactly $k$ changes to the sequence $a$. It is guaranteed that $k$ does not exceed the sum of $a$. In each change:</p><ul> <li> Choose an integer $i$ ($0 \le i &lt; n$) such that $a_i &gt; 0$, and perform $a_i := a_i - 1$. </li></ul><p>Then Ecrade will perform the following three operations sequentially on $a$ and $b$, which constitutes one round of operations:</p><ol> <li> For each $0 \le i &lt; n$: $t := \min(a_i, b_i), a_i := a_i - t, b_i := b_i - t$; </li><li> For each $0 \le i &lt; n$: $c_i := a_{(i - 1) \bmod n}$; </li><li> For each $0 \le i &lt; n$: $a_i := c_i$; </li></ol><p>Ecrade wants to know the minimum number of rounds required for all elements in $a$ to become equal to $0$ after exactly $k$ changes to $a$.</p><p>However, this seems a bit complicated, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $k$ ($1\le n\le 2\cdot 10^5$, $0\le k\le 2\cdot 10^{14}$).</p><p>The second line of each test case contains $n$ integers $a_0, a_1, \ldots, a_{n - 1}$ ($1 \le a_i \le 10^9$).</p><p>The third line of each test case contains $n$ integers $b_0, b_1, \ldots, b_{n - 1}$ ($1 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$. It is also guaranteed that in each test case the sum of $a$ does not exceed the sum of $b$, and that $k$ does not exceed the sum of $a$.</p></div><div class="output-specification"><p>For each test case, output the minimum number of rounds required for all elements in $a$ to become equal to $0$ after exactly $k$ changes to $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$, $k$ ($1\le n\le 2\cdot 10^5$, $0\le k\le 2\cdot 10^{14}$).</p><p>The second line of each test case contains $n$ integers $a_0, a_1, \ldots, a_{n - 1}$ ($1 \le a_i \le 10^9$).</p><p>The third line of each test case contains $n$ integers $b_0, b_1, \ldots, b_{n - 1}$ ($1 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$. It is also guaranteed that in each test case the sum of $a$ does not exceed the sum of $b$, and that $k$ does not exceed the sum of $a$.</p>

## Output

<p>For each test case, output the minimum number of rounds required for all elements in $a$ to become equal to $0$ after exactly $k$ changes to $a$.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
8
3 0
1 1 4
5 1 4
4 0
1 2 3 4
4 3 2 1
4 0
2 1 1 2
1 2 2 1
8 0
1 2 3 4 5 6 7 8
8 7 6 5 4 3 2 1
3 6
1 1 4
5 1 4
4 1
1 2 3 4
4 3 2 1
4 1
2 1 1 2
1 2 2 1
4 2
2 1 1 2
1 2 2 1
```




```output1
1
4
4
8
0
2
2
1
```



## Note

<p>In the fifth test case, all elements in $a$ become $0$ after exactly $6$ changes.</p><p>In the sixth test case, Ecrade can do exactly one change to $a_3$, then $a$ will become $[1,2,2,4]$.</p><ul> <li> After the first round, $a=[3,0,0,0],b=[3,1,0,0]$; </li><li> After the second round, $a=[0,0,0,0],b=[0,1,0,0]$. </li></ul><p>In the seventh test case, Ecrade can do exactly one change to $a_4$, then $a$ will become $[2,1,1,1]$.</p><ul> <li> After the first round, $a=[0,1,0,0],b=[0,1,1,0]$; </li><li> After the second round, $a=[0,0,0,0],b=[0,0,1,0]$. </li></ul>
