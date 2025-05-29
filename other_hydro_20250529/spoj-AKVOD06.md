<p>Cartman and Butters are playing a simple game. They have ¡°N¡± boxes and each box has some amount of money inside it. The boxes are numbered as 1, 2 up to N. In each turn a player can remove a maximum of X(i) amount of money from box i. Inititally the value of X(i) ( 1 &lt;= i &lt;= N) is ¡°Z¡± for all the boxes. At any point a player can select the box i and a value K ( 1 &lt;= K &lt;= X(i)) and remove K amount of money from the box i and update the value of X(i) = K. That means at any point, the amount of money removed from the box can not exceed the amount of money removed from the same box previously. Now let us suppose that both the players play optimally and Cartman takes the first turn. If at any point a player can not remove any money from any box then he loses. Can you predict who will win the game?</p>
<h3>Input</h3>
<p>The first line will contain "T" the no. of test cases. Then "T" test cases follow. The first line of each test case will contain two integers "N" and "Z". The next line will contain "N" integers Ai (1 &lt;= i &lt;= N), where Ai denotes the amount of money in ith box.</p>
<h3>Output</h3>
<p>For each test case, print the name of winner "Cartman" or "Butters" in a separate line (without quotes).&nbsp;</p>
<h3>Constraints</h3>
<div>1 &lt;= T &lt;= 100</div>
<div>1 &lt;= N &lt;= 50</div>
<div>1 &lt;= Z &lt;= 10^4</div>
<div>1 &lt;= Ai &lt;= 1000</div>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 121px; width: 1px; height: 1px; overflow: hidden;">4</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 121px; width: 1px; height: 1px; overflow: hidden;">1 1</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 121px; width: 1px; height: 1px; overflow: hidden;">2 4</div>4</pre>
<pre>1 1
2
2 2
3 3
4 8
3 8 5 10
5 10
8 5 10 20 15
<strong><br></strong></pre>
<pre><strong>Output:</strong>
</pre>
<pre>Butters</pre>
<pre>Butters</pre>
<pre>Cartman</pre>
<pre>Cartman</pre>