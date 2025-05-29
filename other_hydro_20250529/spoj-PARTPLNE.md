<p>You are given the coordinates of 4*K+5 points on a plane such that no three of them are collinear. You need to select five points from these : a central point O and four arm points A,B,C,D such that:</p>
<ul>
<li>Rays from the centre to the arm points divide the plane into four regions containing an equal number of points </li>
<li>None of the four central angles is a reflex angle </li>
<li> Sum of absolute values of the cotangents of the central angles is as low as possible </li>
</ul>
<p>&nbsp;</p>
<p>If it is possible to choose points satisfying this condition, output the lowest possible value for the sum of absolute values of the cotangents of the central angles. Otherwise report that it is not possible.</p>
<h3>Input</h3>
<p>The first line of input contains T(&lt;=4), the number of test cases. Following this are the descriptions of the T test cases.</p>
<p>The first line in the description of each test case gives K(&lt;=100). Following this are 4*K+5 lines giving the x and y coordinates of each point separated by a space (0&lt;=x,y&lt;=10<sup>6</sup>)</p>
<h3>Output</h3>
<p>For each test case output in a different line the minimum sum of absolute values of the cotangents of the central angles, with six digits after the decimal point. If the division cannot be done in the manner explained, print Impossible</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>0<br>0 0<br>0 1<br>1 1<br>1 0<br>2 3<br>0<br>0 0<br>2 0<br>0 1<br>2 1<br>1 2<br><br><strong>Output:</strong><br>4.500000<br>Impossible<br></pre>