<p>You are given an array of integer. You have to find the sum of all possible subsuquences sum of the array. For example: The given array of length n = 3 is {1,2,3}. All the sequence of this array with the corresponding array Summations are:</p>
<table style="width: 638px;" border="1" cellspacing="0" cellpadding="0" align="left">
<tbody>
<tr>
<td width="319" valign="top">
<p align="center">Subsequence</p>
</td>
<td width="319" valign="top">
<p align="center">Summation</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{}&nbsp;</p>
</td>
<td width="319" valign="top">
<p align="center">0</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{1}</p>
</td>
<td width="319" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{2}</p>
</td>
<td width="319" valign="top">
<p align="center">2</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{3}</p>
</td>
<td width="319" valign="top">
<p align="center">3</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{1,2}</p>
</td>
<td width="319" valign="top">
<p align="center">3</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{1,3}</p>
</td>
<td width="319" valign="top">
<p align="center">4</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{2,3}</p>
</td>
<td width="319" valign="top">
<p align="center">5</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">{1,2,3}</p>
</td>
<td width="319" valign="top">
<p align="center">6</p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p align="center">Total</p>
</td>
<td width="319" valign="top">
<p align="center">24</p>
</td>
</tr>
</tbody>
</table>
<p><br class="_<span id=">&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The answer &nbsp;is 24.</p>
<p><span style="font-size: 11.7px;"><strong><span style="font-size: 11.7px; font-weight: bold;">Input</span></strong></span></p>
<p>The first line of input will contain the test case <strong>T (1 &lt;= T &lt;=&nbsp;10)</strong>.There will be two lines for each test case. First line will contain the value of <strong>n(1&lt;=n&lt;=1000)</strong> and the next line will contain the array elements space sperated intergers. Each integer will be between 1 and 1000000000.</p>
<p><strong><span style="font-size: 1.17em;">Output</span></strong></p>
<p><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">For each case of input, output the answer of the problem in the format "</span><strong>Case X: Y</strong><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">" where&nbsp;</span><strong>X</strong><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">&nbsp;denotes the number of test case and&nbsp;</span><strong>Y</strong><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">&nbsp;denotes the answer.&nbsp;</span><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">Answer could be very large so output the answer modulo&nbsp;</span><strong>100000007</strong><span style="color: #333333; font-family: &quot;Open Sans&quot;, Tahoma, Geneva, Verdana, sans-serif; font-size: 14px;">.</span></p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<p>2</p>
<p>3</p>
<p>1 2 3</p>
<p>3</p>
<p>4 1 2</p>
<p><strong>Output:</strong></p>
<p>Case 1: 24</p>
<p>Case 2: 28</p>
<p>&nbsp;</p>