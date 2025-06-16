<p>In order to help terraform Mars, astronauts have brought (among other things) N (0&lt;=N&lt;5) young, healthy pineapple plants.</p>
<p>This particular type of pineapple reproduces asexually in the following way:</p>
<ol>
<li>A single pineapple plant produces K (0&lt;=K&lt;15) new pineapple in one growing season. </li>
<li>At the end of the growing season, the new pineapples are adults, and the old ones are dead. </li>
<li>Increased levels of radiation have a P (0&lt;=P&lt;=1) chance of sterilizing any new pineapple that develops on Mars.  This probability is independent for each pineapple. </li>
</ol>
<p>What is the probability that the pineapple population will never die out?</p>
<h3>Input</h3>
<p>The first line is the number of test cases (no more than 10^5). Each of the following lines describes a test case. The integers N and K and the decimal number P are separated by single spaces.</p>
<h3>Output</h3>
<p>There will be one line for each test case.  Each line will have the probability of eventual survival in percent, to two decimals, followed by the percent sign.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 3 0.6666666666666666
1 3 0.65
1 1 0
1 0 1
3 4 0.7101634622811129

<strong>Output:</strong>
0.00%
13.83%
100.00%
0.00%
70.94%
</pre>