<p>You are given a set of N sticks and are required to partition them into groups of exactly 3 sticks each. While doing so, you can leave out any number of sicks out of these groups (in particular, no groups may be formed). One condition needs to be met: sticks in each group need to form a triangle. A triangle can be constructed if sum of any two sticks lengths is greater than the third length.
</p><p>Your are required to partition the sticks so that the sum of triangle areas from all the groups is maximized.</p>
<p><br></p>

<h3>Input</h3>
<p>Very first line of the input contains integer T: number of test cases (1 &lt;= T &lt;= 5).</p>
<p>For each test case, first line contains integer N: number of sticks. (1 &lt;= N &lt;= 15).</p>
<p>Second line contains N space separated integers: the lengths l<sub>i</sub> of the sicks. (1 &lt;= l<sub>i</sub> &lt;= 10^3,  1  &lt;= i &lt;= N).&nbsp;</p>
<p><br></p>

<h3>Output</h3>
<p>For each test case, output the maximal area in a separate line. Round value to exactly 6 decimal places. <b>Always</b> print exactly 6 decimal places.</p>
<p><br></p>

<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>3<br>7 8 5 <br>4<br>7 8 6 3 <br>3<br>7 2 1<br><br><strong>Output:</strong><br>17.320508<br>20.333163<br>0.000000</pre>