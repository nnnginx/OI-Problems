<p>Given N distinct points in a plane, a point (x1, y1) is said to be dominating another point (x2, y2) if x1&gt;=x2 and y1&gt;=y2.</p>
<p>The Dominance of a point is the absolute difference between 2 quantities ¨C no. of points dominated by this point and no. of points not dominated by this point. <strong>(excluding itself)</strong></p>
<p>A Weird point is the point whose Dominance value is greater than or equal to a threshold value ¡®k¡¯. Find the no. of such Weird Points among those N given points.</p>
<h3>Input</h3>
<p>First line gives T, the no. of test cases.</p>
<p>Each test case consists of 2 integers in first line, N and K, as specified above.</p>
<p>Next N lines give the coordinates of N points in the plane. ¡°Xi¡± and ¡°Yi¡± are space separated.</p>
<h3>Output</h3>
<p>Output T lines, each containing the required answer.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10<br> 1&lt;=N&lt;=10^5<br> 1&lt;=Xi, Yi&lt;=10^9<br> 0&lt;=K&lt;=N</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1</pre>
<pre>4 2</pre>
<pre>3 1<br>7 5<br>2 8<br>6 7</pre>
<pre><strong>Output:</strong><br>2<br><br></pre>
<p><span style="font-size: small;"><strong>Problem Statement and Test Cases has been updated 2012-05-17  18:10:00</strong>.</span></p>