<p>&nbsp;</p>
<p>A map consists of N checkpoints (numbered from 1 to N)&nbsp;connected by M one way roads. A thief is at checkpoint S. He wants to move to checkpoint D. The police, guessing that the thief will move through the route that takes him the least time to&nbsp;reach D from S, have called for security alerts to be placed in all the roads of all such routes. The thief wants to reach D without passing through any of those security alerted roads in the least possible time.&nbsp;If there are multiple such routes, he wants to travel so as to cross a minimum number of checkpoints. Find the minimum time required by the thief to reach D from S, the&nbsp;minimum number&nbsp;of checkpoints in such a route and the number of such routes available. Since the number of such routes may be huge, print the number of such routes modulo 1000000007.</p>
<p><strong>Input</strong></p>
<p>The first line of the input consists of a single integer t representing the number of test cases(1&lt;=t&lt;=300)<br>The first line of each test case consists of two integers N, M where N is the number of checkpoints and M is the number of roads. (1&lt;=N &lt;= 500 and 1&lt;=M &lt;= 10^4)<br>The next M lines consist of three integers x,y,t&nbsp;where x and y represent that the road can be used to travel to checkpoint y from checkpoint x in time t (t &lt;= 100) (1&lt;=x,y&lt;=N)</p>
<p>The last line contains S and D (source and Destination).</p>
<h3>Output</h3>
<p style="text-align: justify;">For each test Case, output a single line containing 3 integers x,y,z. Where x is the least amount of time needed to travel from S to D without using any of the security alerted roads, y is the minimum number of checkpoints in such a route and z is the number of such routes modulo 1000000007. If there is no such path print -1.</p>
<p style="text-align: justify;">&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>3 3</pre>
<pre>1 3 2</pre>
<pre>1 2 2</pre>
<pre>3 2 4</pre>
<pre>1 2

<strong>Output:</strong>
6 3 1</pre>