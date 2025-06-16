<p>In the future world, you have moved into the space colony, and will be using a flying disc which moves in three dimensions as a vehicle. You have been assigned with buying the parts to form 'N' sets of computer from the shops in the colony. Each set of computer consists of 3 parts: monitor, keyboard, and CPU. Because the parts available at one shop may not be enough for the 'N' computers and the budget is limited, you have to design a navigation system for the flying disc such that the total cost of navigation is minimized. You know the exact coordinates of the 'M' available shops and the number of the parts available at each store. Assume that the route from a shop to every other shop will have no obstacles, thus a straight path is always possible, the flying disc contains unlimited storage space, and the parts at each store are free. Let the trip terminate when all parts needed are collected.&nbsp;</p>
<p>Let shop/position A has coordinate (X1, Y1, Z1) and shop/position B has coordinate (X2, Y2, Z2), the navigation cost between the two shops/positions is calculated by the formula (X1-X2)^2 + (Y1-Y2)^2 + (Z1-Z2)^2.</p>
<h3>Input</h3>
<p>The first line contains the integer 'N': the number of the required sets of computer.</p>
<p>The second line contains three integers 'X', 'Y', 'Z': the initial position of the spaceship in the form of coordinates (X, Y, Z)</p>
<p>The third line contains the integer 'M': the total number of shops in the colony</p>
<p>There follows 2M lines: the information for each shop in the colony, where two lines are responsible for the information of one shop.</p>
<p>The first of these two lines contains three integers 'Xi', 'Yi', 'Zi', the position of the shop in the form of coordinates (X, Y, Z)</p>
<p>The second of these two lines contains three integers 'Mi', 'Ki', 'Ci', the number of monitors, keyboards, and CPUs, respectively, available at the shop.</p>
<p>It is guaranteed that it is sufficient to build 'N' sets of computers from all parts of every shop combined.</p>
<h3>Output</h3>
<p>One line containing the minimum navigation cost from the initial position to the end of the trip.</p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= 'N' &lt;= 20</p>
<p>0 &lt;= 'X', 'Y', 'Z', 'Xi', 'Yi', 'Zi' &lt;= 500</p>
<p>1 &lt;= 'M' &lt;= 10</p>
<p>0 &lt;= 'Mi', 'Ki', 'Ci' &lt;= 20</p>
<h3>Example</h3>
<pre><strong>Input #1:<br></strong>1<br>0 0 0<br>2<br>10 0 0<br>2 5 7<br>0 10 0<br>0 3 9</pre>
<pre><strong>Output #1:<br></strong>100</pre>
<pre><strong>Input #2:<br></strong>5<br>0 0 0<br>5<br>60 34 56<br>0 5 7<br>90 41 92<br>1 7 8<br>24 61 81<br>6 8 8<br>41 86 70<br>5 6 7<br>46 97 85 <br>9 2 4</pre>
<pre><strong>Output #2:<br></strong>10542</pre>