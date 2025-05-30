<p>In a billiard table with horizontal side <b>a</b> inches and vertical side <b>b</b> inches, a ball is launched from the middle of the table. After <b>s</b> &gt; 0 seconds the ball returns to the point from which it was launched, after having made <b>m</b> bounces off the vertical sides and <b>n</b> bounces off the horizontal sides of the table. Find the launching angle <b>A</b> (measured from the horizontal), which will be between 0 and 90 degrees inclusive, and the initial velocity of the ball.</p>
<p>
Assume that the collisions with a side are elastic (no energy loss), and thus the velocity component of the ball parallel to each side remains unchanged. Also, assume the ball has a radius of zero. Remember that, unlike pool tables, billiard tables have no pockets.</p>
<h3>Input</h3>
<p>Input consists of a sequence of lines, each containing five nonnegative integers separated by whitespace. The five numbers are: <b>a</b>, <b>b</b>, <b>s</b>, <b>m</b>, and <b>n</b>, respectively. All numbers are positive integers not greater than 10000.</p>
<p>
Input is terminated by a line containing five zeroes.</p>
<h3>Output</h3>
<p>For each input line except the last, output a line containing two real numbers (accurate to two decimal places) separated by a single space. The first number is the measure of the angle <b>A</b> in degrees and the second is the velocity of the ball measured in inches per second, according to the description above.</p>
<h3>Example</h3>

<pre><b>Input:</b>

100 100 1 1 1
200 100 5 3 4
201 132 48 1900 156
0 0 0 0 0

<b>Output:</b>

45.00 141.42
33.69 144.22
3.09 7967.81
</pre>