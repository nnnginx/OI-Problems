<p>Anne and Brenda found some cookies scattered on the lattice points in the 2D coordinate system. They agreed to divide them in the following manner.</p>
<p>First, Anne draws a vertical line (that is, a line with the equation x = c, for any real number c) somewhere in the plane. Then Brenda draws a horizontal line (y = d) somewhere in the plane. Now they have divided the plane in four quadrants.</p>
<p>Anne gets all the cookies lying in the upper right and the lower left quadrant, and Brenda gets all the cookies lying in the upper left and the lower right quadrant. Cookies which lie on the vertical or the horizontal line are ignored.</p>
<p>Anne's goal is to maximize the number of cookies she gets, knowing that Brenda plays optimally (in order to maximize her number of cookies).</p>
<h3>Input</h3>
<p>In the first line of input there is an integer T (1 ¡Ü T ¡Ü 600), the number of test cases.</p>
<p>Each test case starts with an integer N (1 ¡Ü N ¡Ü 1000), the number of cookies. In the next N lines there are coordinates (Xi, Yi) of the cookies, integers in the interval [1, 1000]. There can be multiple cookies at the same point.</p>
<h3>Output</h3>
<p>For each of the T cases, output in a separate line the maximal number of cookies Anne can surely get.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>1 1<br>4 1<br>4 5<br>5 1<br>3 3<br>11<br>7 10<br>7 11<br>7 10<br>7 11<br>6 6<br>5 5<br>4 8<br>1 5<br>1 6<br>1 4<br>7 1<br>
<strong>Output:</strong>
2<br>5</pre>