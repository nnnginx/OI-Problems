<p style="text-align: center;"><strong>Crazy Rows</strong></p>
<p>You are given an <strong>N</strong> x <strong>N</strong> matrix with 0 and 1 values. You can swap any two <em>adjacent</em> rows of the matrix.</p>
<p>Your goal is to have all the 1 values in the matrix below or on the main diagonal. That is, for each X where 1 ¡Ü X ¡Ü N, there must be no 1 values in row X that are to the right of column X.</p>
<p>Return the minimum number of row swaps you need to achieve the goal.</p>
<p>Input</p>
<p>The first line of input gives the number of cases, <strong>T</strong>. <strong>T</strong> test cases follow.<br> The first line of each test case has one integer, <strong>N</strong>. Each of the next <strong>N</strong> lines contains <strong>N</strong> characters. Each character is either 0 or 1.</p>
<p>Output</p>
<p>For each test case, output</p>
<pre>Case #X: K</pre>
<p>where <strong>X</strong> is the test case number, starting from 1, and <strong>K</strong> is the minimum number of row swaps needed to have all the 1 values in the matrix below or on the main diagonal.</p>
<p>You are guaranteed that there is a solution for each test case.</p>
<p>Limits</p>
<p>1 ¡Ü <strong>T</strong> ¡Ü 60</p>
<p>1 ¡Ü <strong>N</strong> ¡Ü 8</p>
<table style="width: 213px; height: 208px;" border="0">
<tbody>
<tr>
<td><span style="font-size: small;">Input<br>&nbsp;</span></td>
<td><span style="font-size: small;">Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> <span style="font-size: small;">3<br> 2<br> 10<br> 11<br> 3<br> 001<br> 100<br> 010<br> 4<br> 1110<br> 1100<br> 1100<br> 1000</span><br> </code></td>
<td valign="top"><span style="font-size: small;"><code> Case #1: 0<br> Case #2: 2<br> Case #3: 4<br> </code></span></td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>