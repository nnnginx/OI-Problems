<p>As King Johnny's temporary indisposition lengthens from days to weeks, and you still hold the office of Regent of Byteland, you begin to feel that acting king is not all that much fun. You encounter various absurdly weird problems. For instance, you find that contrary to your expectations the recent removal of holidays brought about a decrease in the efficiency of the kingdom's workforce.
</p><p>
There appears to be only one rational explanation for all this. It seems that although every holiday occurs every a fixed number of days, the periods between consecutive holidays are long and very irregular. And it is the lack of regularity that is the root of the problem.
</p><p>
So, you decide it is time to tackle the problem once again, and solve it properly this time. 
Your main purpose is to establish an r-day working rhythm (for some integer r). Workers will work for (r-1) days, have a single day off, work for another (r-1) days, and so on. The rhythm must be arranged in such a way that holidays only ever occur on the day off work. Choose exactly k of the n holidays to remove in such a way as to be able to establish a working rhythm of the maximum possible length r.
</p><p>
<b>Solve the problem in at most 4kB of source code.</b>

</p><h3>Input</h3>
<p>The first line of input contains a single integer t&lt;=100 - the number of test cases. t test case descriptions follow.
</p><p>
For each test case, the first line contains two space separated integers n k (1&lt;=k &lt; n&lt;=100), denoting the total number of holidays and the number of holidays to be removed. The next line contains n space separated integers, the i-th being t<sub>i</sub> (1&lt;=t<sub>i</sub>&lt;=10<sup>18</sup>) - the number of days every which the i-th holiday occurs.
</p><h3>Output</h3>
<p>For each test case, output one line containing an increasing sequence of exactly k integers - the numbers of the holidays to be removed (holidays are numbered in the input order from 1 to n).

</p><h3>Example</h3>

<pre><b>Input:</b>
2
6 4
1 3 4 5 6 1
8 4
200 125 200 999 380 500 200 500

<b>Output:</b>
1 3 4 6
2 4 5 6
</pre>
<p>
(In the first test case r is equal to 3 days, in the second case it is equal to 100 days. For the second test case the output '1 2 4 5', '2 3 4 5', '2 4 5 6', '2 4 5 7' or '2 4 5 8' is also correct.)

</p>