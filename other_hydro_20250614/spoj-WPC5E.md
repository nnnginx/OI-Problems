<p><span style="font-size: small;">Each galaxy 'i' in the universe is assigned a unique position in the universe given by A(i), for the ith galaxy.&nbsp;</span><span style="font-size: small;">It is known that the distance between 2 galaxies is given as Dist (i,j) = ( |i^2 - j^2| + |A(i)^2 - A(j)^2| ). </span></p>
<p><span style="font-size: small;">The events are held in a host galaxy, and every other galaxy has to travel to that galaxy to participate. For this, of course, the organizers have to pay the galaxy for their transportation, lodging and daily expenses. The organizers wonder, what could be the maximum transportation expenses that they have to pay?</span></p>
<p><span style="font-size: small;">Help them by finding <strong>MAX</strong>(Dist (i,j)).</span></p>
<p><strong>Input</strong>:</p>
<p>First line contains a single integer T, denoting the number of Test Cases.</p>
<p>Each Test Case contains 2 lines. 1st line containing a single number ¡¯n¡¯ denoting the number of galaxies (numbered 1 to n).</p>
<p>2nd line contains ¡¯n¡¯ space separated integers signifying A(i) for 1&lt;=i&lt;=n.</p>
<p>&nbsp;</p>
<p><strong>Warning</strong>: Fast IO may be needed in some languages.</p>
<p>&nbsp;</p>
<p><strong>Output</strong>:</p>
<p>T lines, each containing an Integer, the answer to the corresponding test case.</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong>:</p>
<p>1 &lt;= T &lt;= 10</p>
<p>2 &lt;= n &lt;= 10^5</p>
<p>1 &lt;= A(i) &lt;= 10^9</p>
<p>&nbsp;</p>
<p><strong>Time Limit</strong>: 2 seconds</p>
<p>&nbsp;</p>
<p><strong>Example</strong>:</p>
<p>&nbsp;</p>
<p><strong>Input</strong>:</p>
<p>1</p>
<p>2</p>
<p>4 3</p>
<p>&nbsp;</p>
<p><strong>Output</strong>:</p>
<p>10</p>
<p>&nbsp;</p>
<p><strong>Explanation</strong>: Dist(i,j) is maximum for i=1, j=2.</p>
<p><span style="font-size: small;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The events are held in a host galaxy, and every other galaxy has to travel to that galaxy to participate. For this, of course, the organizers have to pay the galaxy for their transportation, lodging and daily expenses. The organizers wonder, what could be the maximum transporatation expenses that they would have to pay?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help them find out by finding MAX (Dist (i,j))</div>
<p>&nbsp;</p>