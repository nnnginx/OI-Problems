<p><img src="./22707/file/TOe3RA3z.png" style="float:left">There is a competition of flying hamsters in Hamsterburg. Each competing hamster is thrown from a sling. The initial speed of the hamsters is V0 m/s. Free fall acceleration is g = 10 m/s2. There is no air friction. The size of the hamster and the sling are negligible. When the hamster is thrown from the sling its altitude is 0 meters. There is a number of vertical gates in the air. Each gate has a lower and an upper bound. If we mark the points directly under each of the gates on the ground 每 those points are positioned in one line and on one side from the starting point. A hamster gets as many points as the amount of gates he flies through. You have to calculate the maximal amount of points that a hamster can get in one flight. It is considered that a hamster flies through the gate if he touches the bounds of the gate during the flight or flies between the bounds.
</p><div style="clear:both">&nbsp;</div> 

<h3>Input</h3>
<p>The first line of the input contains number 0 &lt; t &lt;= 10 the amount of test cases. The description of each test case follows. Each test starts with two integers 0 &lt; V0 &lt;= 1000 每 the initial speed of the hamster ans 0 &lt; n &lt;= 20000 每 the total amount of gates. Each of the next n lines contains the description of one of the gates: three integers 0 &lt; x &lt;= 10000 每 the distance from the starting point to the point directly under the gate, 0 &lt; y1 &lt;= y2 &lt;= 10000 每 lower and upper bound of the gate.

</p><h3>Output</h3>
<p>For each test case output the maximal amount of gates a hamster can fly through in one flight on a separate line.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
10 2
3 1 2
3 2 3
10 3
1 1 1
2 2 3
3 4 6
10 3
1 1 2
2 3 4
3 5 6

<b>Output:</b>
2
1
2

</pre>