<p>We call a sequence of n non-negative integers <strong>A</strong>, awesome if there exists some positive integers <strong>x &gt; 1</strong> such that each element <strong>Ai </strong>in A (where <strong>0 &lt;= i &lt; n</strong>) is evenly divisible by <strong>x</strong>. Recall that <strong>a</strong> evenly divides <strong>b</strong> if there exists some integers <strong>c</strong> such that <strong>b = a*c</strong>.</p>
<p>&nbsp;</p>
<p>Given an awesome sequence, <strong>A</strong> and a positive integer <strong>k</strong>, find and print the maximum integer <strong>L</strong>, which satisfies the following conditions:</p>
<ol>
<li><strong>0 &lt;= L &lt;= K</strong></li>
<li>A U {L} is also awesome. (<strong>U</strong> is union operator)</li>
</ol>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the integer <strong>t</strong> denoting the number of test cases. The next line contains two space-separated positive integers, <strong>n</strong> (length of the sequence <strong>A</strong>) and <strong>k</strong> (the upper bound of answer <strong>L</strong>).</p>
<p>The third line contains <strong>n</strong> space separated positive integers describing the elements of <strong>A</strong>.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>For each test case, Print the value of <strong>L</strong> in a single line (where <strong>L</strong> is the maximum integer &lt;= k and A U {L} is also awesome). As 0 is evenly divisible by any <strong>x &gt; 1</strong>, there will always be an answer. &nbsp;&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Constraints: </strong></p>
<p>1 &lt;= t &lt;= 12</p>
<p>1 &lt;= n &lt;= 100000</p>
<p>1 &lt;= k &lt;= 1000000000</p>
<p>1 &lt;= Ai &lt;= 1000000000</p>
<p>&nbsp;</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="312" valign="top">
<p>Sample Input</p>
</td>
<td width="312" valign="top">
<p>Sample Output</p>
</td>
</tr>
<tr>
<td width="312" valign="top">
<p>2</p>
<p>3 5</p>
<p>2 6 4</p>
<p>1 5</p>
<p>7</p>
</td>
<td width="312" valign="top">
<p>4</p>
<p>0</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>