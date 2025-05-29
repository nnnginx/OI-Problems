<p>&nbsp;&nbsp; Byteland is a ficticious city commonly mentioned here on SPOJ.</p>
<p>&nbsp;&nbsp; An ancient legend tells that bytelandians lived in a simple town, just like the Old Western California, where there was just a single straight road of about 500 Meters and all houses, bars and hotel had the road in front of them. In Byteland, although there is a small difference, here, including the Main Road, each house has its own road that connects to the main road, but according to the law, each particular road need to be perpendicular to the main road.</p>
<p>&nbsp;&nbsp; So their world can be abstracted as a two-dimensional grid with integer  coordinates. The main road is the x-axis and houses are points connected  perpendicularly to the x-axis (in both the positive and negative y  directions).</p>
<p>&nbsp;&nbsp; In this particular city, if a person A needs to visit any other person B, he needs to walk along the street that connects his home to the main road until it reaches the main road, then walk through the main road up to the street that comes from the other home, and then walk this street to B's home. But in the case their homes are in the same street, they only need to walk the segment that connects their houses.</p>
<p>&nbsp;&nbsp; The distance between two persons home is defined as:</p>
<p>1)If two homes have the same 'x' coordinate. The distanc<span style="font-size: x-small;">e bet</span>ween them is the absolute difference between their 'y' coordinates. (this is the case where they live in the same street)</p>
<p>2)Otherwise, the distance is the distance between Person A<sub> </sub>and the main road + the distance between Person B and the main road + the absolute difference between their 'x' coordinates.</p>
<p>Here are 3 persons, one at (1,1), other at (1,4), and the last one at (4,1). This is the first example.</p>
<table style="width: 258px; height: 254px;" border="0">
<tbody>
<tr>
<td>
<table border="0">
<tbody>
<tr>
<td><br></td>
</tr>
<tr>
<td>
<table border="0">
<tbody>
<tr>
<td colspan="2"><img src="./23816/file/rAKi1snw.png" alt=""></td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td align="center">&nbsp;</td>
<td>&nbsp;</td>
</tr>
<tr>
<td>&nbsp;</td>
<td>&nbsp;</td>
</tr>
</tbody>
</table>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><span style="font-size: x-small;">&nbsp;&nbsp;<span style="font-size: small;"> The government is about to make a bold decision that will make the lives  of the bytelandians easier. They will minimize the maximum distance between  any pair of persons by moving the main road to a horizontal line y = N,  where N is an integer. If the main road is already at the optimal position,  it will not be moved.</span></span></p>
<p style="text-align: left;"><span style="font-size: small;">&nbsp;&nbsp; You will be given the 'x' and 'y' coordinates of the houses, print the maximum distance between any pair of persons after the main road is moved to the optimal position.</span></p>
<h3>Input</h3>
<p>The first line is <strong>T</strong> (3 ¡Ü <strong>T</strong> ¡Ü 1,000), the number of test cases, then <strong>T</strong> test cases follows.</p>
<p>Each test case starts with <strong>N</strong> (2 ¡Ü <strong>N</strong> ¡Ü 50), the number of persons in byteland.</p>
<p>then <strong>N</strong> lines, each one with two integers separated by a space.</p>
<p>Each one of these integers is the x and y coordinates, respectively, of a bytelandian home.</p>
<p><strong>Constraints:</strong></p>
<p>-The absolute value of each <strong>x</strong> and <strong>y</strong> coordinate will be between 0 and 10<sup>9</sup>, inclusive.</p>
<h3>Output</h3>
<p>For each test case print out the required distance in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>3<br>1 4<br>4 1<br>1 1<br>5<br>-1 -1<br>-2 3<br>-1 -3<br>0 0<br>2 3<br>4<br>1 1<br>1 10<br>1 100<br>1 1000<br><br><strong>Output:</strong><br>6<br>9<br>999</pre>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 482px; width: 1px; height: 1px; overflow: hidden;">The government is about to make a bold decision that will make the lives  of the monkeys easier. They will minimize the maximum distance between  any pair of monkeys by moving the ground to a horizontal line y = N,  where N is an integer. If the ground is already at the optimal position,  it will not be moved.</div>