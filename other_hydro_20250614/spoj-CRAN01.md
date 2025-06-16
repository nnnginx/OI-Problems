<p>Penny started studying in a community college. However she did not tell Leonard about this because she did not want Leonard helping her at every point in her studies. This went well until the professor ordered her to perform an advanced experiment. In this experiment she was given an advanced microbiological specimen. This specimen is placed in an n X m size grid which is divided into 1 X 1 cells.</p>
<p>It expands according to following rules.</p>
<p>If at time t, the specimen occupies &nbsp;(x ,y), then at time t+1 it can expand to at most any two cells out of (x+1,y), (x-1,y), (x,y+1), (x,y-1).</p>
<p>For example if at t = 0 sec if the specimen occupies (4, 5), then at time t = 1 sec, the state of the grid can be any of the following</p>
<p>1. specimen at (4,5), (5,5) and (3,5).</p>
<p>2. specimen at (4,5), (5,5) and (4,6).</p>
<p>3. specimen at (4,5), (5,5) and (3,4).</p>
<p>4. specimen at (4,5), (3,5) and (4,6).</p>
<p>5. specimen at (4,5), (3,5) and (4,4).</p>
<p>6. specimen at (4,5), (4,6) and (4,4).</p>
<p><strong>Note-</strong> At t= 2 sec, it can expand from all the points that the specimen occupied at t= 1.</p>
<p>The professor asks penny to find the minimum time it takes for the specimen to fill the entire grid.</p>
<p>Since penny is not so smart at math and she can't ask Leonard to help her, she turns to you for help and to find the solution to above problem.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>T - The number of test cases.</p>
<p>n m - number of row and columns in the grid.</p>
<p>x y - coordinate of the initial position of the specimen.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The minimum time in seconds it takes for specimen to fill in the entire grid.</p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><strong>Constraints</strong></span></p>
<p>1 &lt;= T &lt;= 50</p>
<p>1 &lt;= n, m &lt;= 500</p>
<p>1 &lt;= x &lt;= n</p>
<p>1 &lt;= y &lt;= m</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1 1<br>1 1<br>10 10<br>6 4

<strong>Output:</strong>
0<br>11</pre>