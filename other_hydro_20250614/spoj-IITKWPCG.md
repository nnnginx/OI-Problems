<p>&nbsp;&nbsp;&nbsp;&nbsp; Once upon a time there lived a king in a far far country. In the country, there are n cities and m roads. He was severly attacked by his enemy. The enemy damaged all the cities of King's country. As the roads between the cities had been damaged, the King wanted to repair those. So he decided to launch a tender for this. <br><br>&nbsp;&nbsp;&nbsp;&nbsp; As King's country is a well managed country. By well managed country, we mean that it is possible to go from each city to any other city. But now as the city has been destroyed by enemies, all the roads are broken, the king will like to rebuild the roads in such a way that it is still a well manged country. <br>&nbsp;&nbsp;&nbsp;&nbsp; <br>&nbsp;&nbsp;&nbsp; Cost of repairing the road in the country is really wierd, it is not addition of costs but it is instead multiplication of those. What it means that if the king decides that he should repair 5 roads, then total cost of repairing those roads will be multiplication of all the 5 costs.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp; As the King's treasure has been damaged by the attack of foreign city, he would like to spend minimum amount of money and that the will want that his country still remains well managed country. Surprisingly the company that was given tender had a rule that all the costs will be in powers of two, as they were really love with binary numbers.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp; As value of the total cost can be really large. We do not want to know the actual cost, instead output number of divisors of the number.</p>
<h3>Input</h3>
<p>T: number of test cases (T &lt;= 5)<br>n and m (n &lt;= 10^5 &amp;&amp; m &lt;= 2 * 10^5)</p>
<p>Next m lines will have a, b, c, which denotes that cities a and b are connected with road of cost c.</p>
<p>(c &gt;= 2 &amp;&amp; c &lt;= 10^18 &amp;&amp; c will always be power of 2) (1 &lt;= a &lt;= n) and (1 &lt;= b &lt;= n)</p>
<h3>Output</h3>
<p>For each test case, output a single line containing a number as stated in the problem..</p>
<p><strong>Example</strong></p>
<p><span style="font-weight: bold;">Input:</span></p>
<p><span style="white-space: pre-wrap;">4</span></p>
<p><span style="white-space: pre-wrap;">2 1</span></p>
<p><span style="white-space: pre-wrap;">1 2 16</span></p>
<p><span style="white-space: pre-wrap;">3 2</span></p>
<p><span style="white-space: pre-wrap;">2 3 32</span></p>
<p><span style="white-space: pre-wrap;">1 2 16</span></p>
<p><span style="white-space: pre-wrap;">3 3</span></p>
<p><span style="white-space: pre-wrap;">2 3 32</span></p>
<p><span style="white-space: pre-wrap;">1 2 16</span></p>
<p><span style="white-space: pre-wrap;">1 3 64</span></p>
<p><span style="white-space: pre-wrap;">5 5</span></p>
<p><span style="white-space: pre-wrap;">1 2 2</span></p>
<p><span style="white-space: pre-wrap;">2 3 2</span></p>
<p><span style="white-space: pre-wrap;">1 3 4</span></p>
<p><span style="white-space: pre-wrap;">3 4 16</span></p>
<p><span style="white-space: pre-wrap;">3 5 8</span></p>
<p><span style="font-weight: bold; white-space: pre-wrap;">Output:</span></p>
<p><span style="white-space: pre-wrap;">5</span></p>
<p><span style="white-space: pre-wrap;">10</span></p>
<p><span style="white-space: pre-wrap;">10</span></p>
<p><span style="white-space: pre-wrap;">10</span></p>