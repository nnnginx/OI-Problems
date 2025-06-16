<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">9 7 5 19 7 2 10 7 2 4&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">16 17 13 2 2 19 14 18 4 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">9 1 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">1 2 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">10 3 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">2 4 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">7 5 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">7 6 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">5 8 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">5 9 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 525px; width: 1px; height: 1px; overflow: hidden;">7 10 1</div>
<p>Ariel is a travelling salesman in his own world. Ariel wants to buy some toys at city <strong>X</strong> and sells them at city <strong>Y</strong> (<strong>X</strong> can be equal to <strong>Y</strong>).<strong>&nbsp;</strong></p>
<p>&nbsp;</p>
<p>His own world forms a weighted tree.</p>
<p>The cost to travel from city <strong>X</strong> to city <strong>Y</strong> is the sum of weight of edge between city <strong>X</strong> and city <strong>Y</strong>.</p>
<p>You are given <strong>A[i]</strong>, <strong>B[i]</strong>.</p>
<p><strong>A[i]</strong> denote the maximum number of toy that Ariel can buy at city <strong>i</strong>.</p>
<p><strong>B[i]</strong> denote the price of buying / selling a toy in city <strong>i</strong>.</p>
<p>Ariel can choose two city. Let it be <strong>X</strong> and <strong>Y</strong>. such that he can buy some toy at city <strong>X</strong>, travel between <strong>X</strong> and <strong>Y</strong>, and sell some toy at city <strong>Y</strong>.</p>
<p>Ariel can only buy some toy at no more than one city, and can only sell some toy at no more than one city.</p>
<p>Help Ariel to maximize his profit.</p>
<h3>Input</h3>
<p>First line contains an integer N.</p>
<p>Second line contains N integer A[i].</p>
<p>Third line contains N integer B[i].</p>
<p>The next N-1 lines contains U V and W, there is an edge between U and V with weight W.</p>
<h3>Output</h3>
<p>One integer that denote maximum profit Ariel can get.</p>
<h3>Constraint</h3>
<p>2 &lt;= N &lt;= 1e5.</p>
<p>1 &lt;= A[i], B[i], W&lt;= 1e9.</p>
<p>1 &lt;= U, V &lt;= N</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>4
10 10 10 10
5 5 5 5
1 2 1
2 3 1
3 4 1</pre>
<pre><strong>Output:</strong>
0</pre>
<pre><strong>Input:</strong>
5
1 9 4 16 5 
20 5 10 15 19 
2 1 6
2 3 6
2 4 7
3 5 4

<strong>Output:</strong>
129</pre>
<pre><strong>Input:</strong>
10
9 7 5 19 7 2 10 7 2 4 
16 17 13 2 2 19 14 18 4 1
9 1 4
1 2 7
10 3 5
2 4 6
7 5 5
7 6 1
5 8 7
5 9 10
7 10 1

<strong>Output:</strong>
290</pre>