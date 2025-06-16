<pre><span style="white-space: normal;"><h2>Array with Hudai Calculation</h2>
<p>You will be given an array A with N integers A[1¡­N]. You will also be given two integers P and K. You need to find a value X [ X can be any value from array A] for which this function will be maximized:</p>
<p>&nbsp;<img title="formula" src="file://EN2awMkf.png" alt="formula" width="622" height="123"></p>
<p>Here ABS means Absolute Value. For example: ABS(-1) is 1, also ABS(1) means 1.</p>
<p>Here MOD means Modulo Operation.&nbsp; W MOD Y will give you the remainder after dividing W by Y.</p><p>And X is any value from the array A.</p>
<p>But we don¡¯t have interest in X, as there will be several X for which the value will be maximized. So we just want the maximum value. Can you find it for us as you are a great programmer on SPOJ ?</p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 5)</strong>, denoting the number of test cases.</p>
<p>Each case starts with a line containing three integers&nbsp;<strong>N</strong>, <strong>P and K</strong>. Then the next line will be consisting of N integers.</p>
<p>1 &lt;= N &lt;= 100000</p><p>1 &lt;= P &lt;= 100</p><p>1 &lt;= K &lt;= 1000000009</p><p>1 &lt;= A[i] &lt;= 2000<br> <br> </p>
<p><strong>Output</strong></p>
<p>For each case, print the case number and the maximum value for the above function with respect to array A.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong>Sample Input</strong></p>
</td>
<td width="319" valign="top">
<p><strong>Output for Sample Input</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p>2</p>
<p>3 1 10</p>
<p>3 1 2</p>
<p>3 2 10</p>
<p>3 1 2</p>
<p>&nbsp;</p>
</td>
<td width="319" valign="top">
<p>Case 1: 3</p>
<p>Case 2: 5</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>N.B: Dataset is huge. Use faster IO like Scanf , Printf</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p></span></pre>