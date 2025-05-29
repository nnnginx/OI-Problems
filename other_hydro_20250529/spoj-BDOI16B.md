<p style="margin-bottom: 0.14in" align="CENTER"><span style="font-size: large;"><strong>Beautiful Factorial Game</strong></span></p>
<p style="margin-bottom: 0.14in">The statement of this problem is very simple. Given two number n and k, you need to find the maximum power of k (i.e. x) such that n! % k^x = 0. Here n! is the notation of n factorial. If you are not familiar with the notation,</p>
<p style="margin-bottom: 0.14in" align="CENTER">n! = 1 * 2 * 3 * 4 * 5 * 6 ¡­.. * n</p>
<p style="margin-bottom: 0in; line-height: 100%"><strong>Input:</strong></p>
<p style="margin-bottom: 0.14in">First line of the input will contain an integer t (1 &lt;= t &lt;= 20) denoting the number of test case. The next t lines contain two integer number n and k as described above.</p>
<p style="margin-bottom: 0in; line-height: 100%"><strong>Constraints:</strong></p>
<p style="margin-bottom: 0in; line-height: 100%">For easy version, 1 &lt;= n &lt;= 10, 2 &lt;= k &lt;= 10</p>
<p style="margin-bottom: 0.14in">For harder version, 1 &lt;= n &lt;= 100000000, 2 &lt;= k &lt;= 100000000</p>
<p style="margin-bottom: 0in; line-height: 100%"><strong>Output:</strong></p>
<p style="margin-bottom: 0.14in">For each test case, print ¡°Case t: x¡± where t is the test case number and x is the maximum power of k for which n! % k^x = 0.</p>
<table style="width: 638px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="304"> <col width="304"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border: 1px solid #000001; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p align="CENTER"><strong>Sample Input</strong></p>
</td>
<td style="border: 1px solid #000001; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p align="CENTER"><strong>Output of sample input</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border: 1px solid #000001; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p style="margin-bottom: 0.14in">2</p>
<p style="margin-bottom: 0.14in">5 2</p>
<p>1000 2</p>
</td>
<td style="border: 1px solid #000001; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p style="margin-bottom: 0.14in">Case 1: 3</p>
<p>Case 2: 994</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0.14in"><br><br></p>
<p style="margin-bottom: 0in; line-height: 100%"><strong>Explanation of the sample:</strong></p>
<p style="margin-bottom: 0in; line-height: 100%">In the first test case, n = 5 and k = 2. So, n! = 120.</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^0 = 0</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^1 = 0</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^2 = 0</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^3 = 0</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^4 = 8</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^5 = 24</p>
<p style="margin-bottom: 0in; line-height: 100%" align="CENTER">n! % 2^6 = 56</p>
<p style="margin-bottom: 0.14in" align="CENTER">n! % 2^7 = 120</p>
<p style="margin-bottom: 0.14in">So, the answer should be 3.</p>
<p style="margin-bottom: 0.14in"><span style="font-size: medium;"><strong>Problem Setter: Rakibul Islam </strong></span></p>
<p style="margin-bottom: 0.14in" align="CENTER"><br><br></p>
<p style="margin-bottom: 0.14in" align="CENTER"><br><br></p>