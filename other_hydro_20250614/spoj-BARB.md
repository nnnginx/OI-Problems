<p>There are N Barbarians living on an unknown island. On the island there are M caves, we can number them 1, 2, ..., M clockwise. When we find
the island, the barbarians are living in N distinct caves numbered C1,C2,...,CN.Every year each barbarian walks out of his cave and goes along the
road,passes Pi caves and then go into that cave.Every Barbarian has a living time: Li years, after Li years the ith barbarian died.</p>
<p>We are surprised to find out that no two barbarians live in one cave in the same year so no conflicts have happened.We are interesting about
the minimum number of caves on the island.</p>
<b>Please note that this problem has a somewhat strict source limit and time limit.</b>
<h3>Input</h3>
<p>The very first line contains a single integer T,the number of test cases.T blocks follow. </p>
<p>For each test case, the first line contains a single integer N(N&lt;=15).N lines follow,each contains 3 integers Ci(1&lt;=Ci&lt;=100),Pi(1&lt;=Pi&lt;=100),Li
(1&lt;=Li&lt;=1,000,000).</p>
<h3>Output</h3>
<p>For each test case, the first and only line contains a single integer M - the answer.You may assume M&lt;=1,000,000.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
3
1 3 4
2 7 3
3 2 1

<b>Output:</b>
6
<b>Hints</b>
-------------------------------------------------
| Year | Barb. No.1 | Barb. No. 2 | Barb. No. 3 |
-------------------------------------------------
|  0   |     1      |      2      |      3      |
-------------------------------------------------
|  1   |     4      |      3      |      5      |
-------------------------------------------------
|  2   |     1      |      4      |    Died     |
-------------------------------------------------
|  3   |     4      |      5      |    Died     |
-------------------------------------------------
|  4   |     1      |    Died     |    Died     |
-------------------------------------------------
</pre>