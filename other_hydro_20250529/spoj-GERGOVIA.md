<p>Gergovia consists of one street, and every inhabitant of the city is a wine salesman. Everyone buys wine from other inhabitants of the city. Every day each inhabitant decides how much wine he wants to buy or sell. Interestingly, demand and supply is always the same, so that each inhabitant gets what he wants.</p>
<p>There is one problem, however: Transporting wine from one house to another results in work. Since all wines are equally good, the inhabitants of Gergovia don't care which persons they are doing trade with, they are only interested in selling or buying a specific amount of wine.</p>
<p>In this problem you are asked to reconstruct the trading during one day in Gergovia. For simplicity we will assume that the houses are built along a straight line with equal distance between adjacent houses. Transporting one bottle of wine from one house to an adjacent house results in one unit of work.</p>
<h3>Input</h3>
<p>The input consists of several test cases.</p>
<p>Each test case starts with the number of inhabitants N (2 ¡Ü N ¡Ü 100000).</p>
<p>The following line contains n integers a<sub>i</sub> (-1000 ¡Ü a<sub>i</sub> ¡Ü 1000).</p>
<p>If a<sub>i</sub> ¡Ý 0, it means that the inhabitant living in the i<sup>th</sup> house wants to buy a<sub>i</sub> bottles of wine. If a<sub>i</sub> &lt; 0, he wants to sell -a<sub>i</sub> bottles of wine.</p>
<p>You may assume that the numbers a<sub>i</sub> sum up to 0.</p>
<p>The last test case is followed by a line containing 0.</p>
<h3>Output</h3>
<p>For each test case print the minimum amount of work units needed so that every inhabitant has his demand fulfilled.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>5<br>5 -4 1 -3 1<br>6<br>-1000 -1000 -1000 1000 1000 1000<br>0<br><br><strong>Output:</strong><br>9<br>9000<br></pre>