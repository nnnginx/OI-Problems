<p>In this problem you will work on a plane, where the natural numbers are arranged in a stair pattern.</p>
<p>Starting on coordinate (2,1) thru (2,23) are the first 23 natural numbers in sequence, 1 is in (2,1), 2 is in (2,2) and so on...,the next 23 natural numbers (24 to 46) are arranged from (2,24) thru (24,24), the next 23 from (25,24) thru (25,46), a stair pattern where each step is 24 numbers high, this pattern continues infinitely.</p>
<p>Y-axis</p>
<p>|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; 48</p>
<p>|&nbsp; 24 25 26 27 . . . 46 47</p>
<p>|&nbsp; 23</p>
<p>|&nbsp;&nbsp; .</p>
<p>|&nbsp;&nbsp; .</p>
<p>|&nbsp;&nbsp; . &nbsp;&nbsp;</p>
<p>|&nbsp; 3</p>
<p>|&nbsp; 2</p>
<p>|&nbsp; 1</p>
<p>_____________________________ X axis</p>
<h3>Input</h3>
<p>You will be given a series of queries that could be one or two integers per line.</p>
<p>The last test case is 0 0.</p>
<p>each integer N, X<sub>i</sub>, Y<sub>i </sub>satisfy: 1 ¡Ü N, X<sub>i</sub>, Y<sub>i</sub>, ¡Ü 10<sup>15</sup>.</p>
<h3>Output</h3>
<p>If the test case is one integer you have to output two comma separated integers denoting the coordinates (x,y) of the selected number, if there are two numbers you have to output one integer that corresponds to the integer that is located in those coordinates, if there is no number with such coordinates, output the string "No Number"</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>2 7<br>3 7<br>0 0<br><br><strong>Output:</strong><br>2, 2<br>7<br>No Number</pre>