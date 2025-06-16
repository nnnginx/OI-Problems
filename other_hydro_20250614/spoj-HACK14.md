<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Aiden Pearce is one of the most famous hackers of all time, just recently he acquired a new powerful teleport that can be used exactly K times before it self-destructs.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">So he decided to rob as many banks as he can from Linearland. Linearland consists of N cities on a 1-Dimensional plane which Aiden can visit, after he¡¯s teleported to some city of Linearland he can begin robbing banks, each city i has a bank that contains G[i] dollars.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The teleportation device is also expensive to use; in order to teleport to some city i he has to pay T[i] dollars but teleportation isn¡¯t his only means of transport he can also visit cities by helicopter which costs W dollars per meter. Aidens initial position is outside Linearland, so, the first city he visits can only be reached by teleportaion.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each city i is situated in position X[i] (which means it¡¯s X[i] meters far from the beginning of Linearland). Aiden isn¡¯t sure that robbing Linearland banks is profitable so he asked you to calculate the maximum amount of money he can earn.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(Aiden can have a negative amount of money at any time).</div>
<p>Aiden Pearce is one of the most famous hackers of all time, just recently he acquired a new powerful teleport that can be used exactly K times before it self-destructs.</p>
<p>So he decided to rob as many banks as he can from Linearland. Linearland consists of N cities on a 1-Dimensional plane which Aiden can visit, after he¡¯s teleported to some city of Linearland he can begin robbing banks, each city i has a bank that contains G[i] dollars.</p>
<p>The teleportation device is also expensive to use; inn order to teleport to some city i he has to pay T[i] dollars but teleportation isn¡¯t his only means of transport he can also visit cities by helicopter which costs W dollars per meter. Aidens initial position is outside Linearland, so, the first city he visits can only be reached by teleportaion.</p>
<p>Each city i is situated in position X[i] (which means it¡¯s X[i] meters far from the beginning of Linearland). Aiden isn¡¯t sure that robbing Linearland banks is profitable so he asked you to calculate the maximum amount of money he can earn.</p>
<p>(Aiden can have a negative amount of money at any time).</p>
<p>Please note that Aiden doesn't need to use all K teleports, and since he is very greedy he will never go to Linearland if his net profit is negative (i.e if he can't get a positive profit he will settle with a good old 0)</p>
<h3>Input</h3>
<p>First T the number of test cases,</p>
<p>For each test case:</p>
<p>3 integers separated by space representing (1 &lt;= N &lt;= 10^3), (1 &lt;= K &lt;= N) and (W &lt;= 10^9).</p>
<p>Then N lines each line consists of 3 integers (0 &lt;= X[i] &lt;= 10^9), (1 &lt;= T[i] &lt;= 10^9), (1 &lt;= &nbsp;G[i] &lt;= 10^9).</p>
<h3>Output</h3>
<p>One line per test case, each with a single integer which is the maximum amount of money.</p>
<pre><strong>Input:</strong>
1
4 1 1
1 1000 100
3 0 10
4 20 3
10 90 0

<strong>Output:</strong>
109
</pre>