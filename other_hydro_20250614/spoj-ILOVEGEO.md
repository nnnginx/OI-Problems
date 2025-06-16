<p>In this Years RoboFest in IUT(International University Of Technology) There a segment called LFR contest. An LFR contest is a contest where the robots have to follow a specific line. The track was bound by a inner and a outer polygon. More clearly the space between the two polygon was track. Now, to make the contest easier, the authority created glass walls along with the lines of the poligons so that no robot gets out of the track. There is a rule that all the robots have to be circular. Given the coordinates of the points of both polygon in consecutive order, Find the biggest diameter possible for a robot so that it does not get stuck anywhere in the track.(does not get stuck between walls.</p>
<h3>Input</h3>
<p>First line of the input contains 0&lt;t&lt;101, number of testcases</p>
<p>then in the next t testcases,</p>
<p>Tach testcase starts with a number 2&lt;N<sub>i</sub>&nbsp;&lt;101 ,number of points of the inner polygon.</p>
<p>Then next N<sub>i</sub>&nbsp;lines contains two integer each, X<sub>i</sub>,Y<sub>i</sub>&nbsp;denoting coordinates of the point in inner polygon</p>
<p>Then comes a number 2&lt;N<sub>o</sub>&lt;101 Number of points in the outer polygon.</p>
<p>Then next N<span style="font-size: 8.33333px;">o</span>&nbsp;lines contains two integer each, X<sub>i</sub>,Y<sub>i</sub>&nbsp;denoting coordinates of the point in the outer polygon.</p>
<p>All coordinates have absolute value no larger than 1000. The points of the polygons can be given in either clockwise or counterclockwise order and the two polygons do not intersect or touch themselves or each other. The outer polygon encloses the inner polygon.</p>
<h3>Output</h3>
<p>For each testcase on a new line print a floating point number rounded upto 6 digits denoting the maximal diameter possible for the robot.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre><strong>2 </strong></pre>
<pre><strong>4 </strong></pre>
<pre><strong>-5 -5 </strong></pre>
<pre><strong>5 -5 </strong></pre>
<pre><strong>5 5 </strong></pre>
<pre><strong>-5 5 </strong></pre>
<pre><strong>4 </strong></pre>
<pre><strong>-10 -10 </strong></pre>
<pre><strong>-10 10 </strong></pre>
<pre><strong>10 10 </strong></pre>
<pre><strong>10 -10 </strong></pre>
<pre><strong>3 </strong></pre>
<pre><strong>0 0 </strong></pre>
<pre><strong>1 0 </strong></pre>
<pre><strong>1 1 </strong></pre>
<pre><strong>5 </strong></pre>
<pre><strong>3 -3 </strong></pre>
<pre><strong>3 3 </strong></pre>
<pre><strong>-4 2 </strong></pre>
<pre><strong>-1 -1 </strong></pre>
<pre><strong>-2 -2</strong></pre>
<pre><strong>Output:</strong></pre>
<pre>5.000000</pre>
<pre>1.414214</pre>