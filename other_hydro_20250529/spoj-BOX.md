<p>There are n boxes on the circle. The boxes are numbered from 1 to n in clock wise order. There are balls in the boxes, and the number of all the balls in the boxes is not greater than n.</p>
<p>The balls should be displaced in such a way that in each box there remains no more than one ball. In one move we can shift a ball from one box to one of it's neighboring boxes.</p>
<p>Write a program that:  reads from the standard input the number of boxes n and the arrangement of balls in the boxes,  computes the minimal number of moves necessary to displace the balls in such a way that in each box there remains no more than one ball,  writes the result in the standard output.</p>
<h3>Input</h3>
<p>The first line of the input file contains an integer t representing the number of test cases. Then t test cases follows. Each test case has the following form:</p>
<ul>
<li> The first line contains one positive integer n - the number of boxes </li>
<li> The second line contains n nonnegative integer separated by single spaces. The i-th number is the number of balls in the i-th box. </li>
</ul>
<h3>Output</h3>
<p>For each test case, output one nonnegative integer - the number of moves necessary to displace the balls in such a way that in each box there remains no more than one ball.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
12
0 0 2 4 3 1 0 0 0 0 0 1

<strong>Output:</strong>
19
</pre>
<h3>Note</h3>
<p>There are two input files.</p>
<p>In the first input file, t=19, n&lt;=1000, time limit=0.1 second;</p>
<p>In the second input file, t=3, n&lt;=200000, time limit=2 seconds.</p>
<p><strong>Warning: large input/output data, be careful with certain languages</strong></p>