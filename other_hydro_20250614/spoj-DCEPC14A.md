<p>DCE Coders admins are way much geekier than they actually seem! Kartik has been following that tradition lately. How? Well, he took the inversion count problem to a whole new level!</p>
<p>Sounds pretty normal to you, huh? Wanna challenge him? Try solving his version of inversion count then!</p>
<p>You are given a 2-d array of integers. You need to find out the inversion count of that array. A pair of integers in the 2-d array counts as an inversion pair (A,B) if and only if:</p>
<ul>
<li>There exists a valid path from top-left corner (0,0) to bottom right corner (r,c) such that A and B integers lie on that path.</li>
<li>A occurs before B on that path.</li>
<li>And, A &gt; B.</li>
</ul>
<p>A valid path is defined as a path that can be traversed from top-left corner (0,0) to bottom-right corner (r,c) by moving only in right or downwards direction, without moving out of the grid.</p>
<p>Are you geekier than Kartik?</p>
<p><strong>Constraints:</strong></p>
<p>0 &lt; R,C &lt;= 300</p>
<p>0 &lt; Ai &lt;= 10^5, where Ai stands for an integer in the array.</p>
<h3>Input</h3>
<p>First line contains space separated 2 integers, R and C, denoting the number of rows and columns.</p>
<p>Next R lines contain C space separated integers representing the 2-d array</p>
<h3>Output</h3>
<p>Output the number of inversion pairs as described in the problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>4 4
</p><p>3 4 2 5
</p><p>1 7 11 16
</p><p>8 9 6 12
</p><p>10 13 15 14</p>

<strong>Output:</strong>
<p>10</p>
</pre>