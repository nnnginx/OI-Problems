<p>Farmer Cream is a businessman that wants to live in the suburbs. He recently bought a little farm in Creamville and wants to earn money from it. After the sell, Farmer Cream has D money a remaining to spend. He's in negotiations with an important firm of farming but he thinks they're not being honest (they're trying to steal some money). He knows the number of fences F in the farm but he doesn't know the number of plots P to farm. The firm is offering a budget B per plot, so he needs to multiply the budget per the number of plots to know the total amount of money to spend. He needs to know if he accepts the contract, for that, he<br>needs to have at least M money to live after the buy. Otherwise, the firm is trying to bankrupt Farmer Cream and take over the farm.</p>
<p>In order to do this. Farmer Cream needs your help. Assuming the fences are lines y = ax + b he only knows three things about them.</p>
<p>&nbsp;</p>
<ol>
<li>There is no point in the farm where 3 or more fences collides. So, in one point of the farm there'll be zero, one or two fences.</li>
<li>There are no parallel fences in the farm. So if we have two fences represented by y1 = a1x1 + b1 and y2 = a2x2 + b2 we assume that a1 &lt;&gt; a2.</li>
<li>All the fences collide with each other</li>
</ol>
<p>&nbsp;</p>
<p style="text-align: center;"><img style="vertical-align: middle;" src="../../../content/henu:ucv2013A" alt="Example with 3 fences and 7 plots" width="225" height="240"></p>
<p>In the example, there are 3 fences and 7 plots.</p>
<h3>Input</h3>
<p>The input contains several test cases, each one corresponding to a different situation. Each test case consists of a single line with four integers D F B M (1 &lt;= F,B,M &lt;= 10^6) and (1 &lt;= D &lt;= 10^18) separated by a single space. D represents the remaining money of Farmer Cream, F represents the number of fences, B represents the budget in Bsf per plot and M represents the minimum amount of money that Farmer Cream needs to live.</p>
<p><br>The end of input is indicated by a test case with D = F = B = M = 0.</p>
<h3>Output</h3>
<p>For each test case, you'll print: "The firm is trying to bankrupt Farmer Cream by X Bsf." where X represents the difference between money to spend plus the money he needs to survive and the money Farmer Cream has. Otherwise, you'll print "Farmer Cream will have Y Bsf to spend." where Y represents the money Farmer Cream will have to spend.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
160 1 70 30<br>500 3 50 100<br>250000 40 300 5000<br>0 0 0 0

<strong>Output:</strong>
The firm is trying to bankrupt Farmer Cream by 10 Bsf.<br>Farmer Cream will have 150 Bsf to spend.<br>The firm is trying to bankrupt Farmer Cream by 1300 Bsf.
</pre>