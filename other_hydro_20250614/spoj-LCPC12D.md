<pre><span style="white-space: normal;"><h2>Description</h2>
<p>Johnny has a map of the gang block which shows the heights of all buildings within the block. The plan is that a helicopter will drop Johnny on the roof of one of the buildings on the boundaries of the block during night. Then Johnny will get to the boss's building by moving to adjacent buildings, vertically or horizontally. Going up severely affects Johnny��s heart, so he can only go to a building which has the same or smaller height as the current building.</p>
<p>Given the gang building block map which shows the heights of all buildings in the block along with the boss building, write a program to help Johnny determine the safest path from any building on the boundary of the block to reach the boss��s building without going up. A path safety is measured by the maximum jump value between any two buildings along the path, where the jump value is the difference between the heights of the two buildings (the building he jumps from and the building he jumps to).&nbsp; The safest path is the path with minimum safety value.</p>
<h2>Input Format</h2>
<h2>The first line of input contains an integer <em>T</em>, the number of test cases. <em>T</em> test cases follow, the first line of each test case contains two integers (1 &lt;= <em>R</em>,<em>C</em> &lt;= 10) the height and the width of the building block. The second line contains two integers (1 &lt;= <em>B<sub>R</sub></em> &lt;= <em>R</em>), and (1 &lt;= <em>B<sub>C</sub></em> &lt;= <em>C</em>), the coordinates of the boss��s building on the map. <em>R</em> lines follows; each line consists of <em>C</em> space separated integers representing the heights of all buildings. A height <em>H</em> of a building satisfies (1 &lt;= <em>H</em> &lt;= 1000).</h2>
<h2>Output Format</h2>
<p>For each test case, output the result using the following format:</p>
<p><strong><em>k</em></strong>. <strong><em>S</em></strong></p>
<p>Where <strong><em>k</em></strong> is the test case number (starting at 1), a single period (.), a single space, and <strong><em>S</em></strong> (the safety value of the safest path) or <strong>"IMPOSSIBLE"</strong> (quotes for clarity) if there is no path to the boss's building.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="284" valign="top">
<h2>Sample Input</h2>
</td>
<td width="284" valign="top">
<h2>Sample Output</h2>
</td>
</tr>
<tr>
<td width="284" valign="top">
<p>2</p>
<p>3 3</p>
<p>2 2</p>
<p>1 7 3</p>
<p>2 6 3</p>
<p>3 5 4</p>
<p>2 2</p>
<p>2 1</p>
<p>2 7</p>
<p>2 6</p>
</td>
<td width="284" valign="top">
<p>1. 1</p>
<p>2. 0</p>
<p>&nbsp;</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p></span></pre>