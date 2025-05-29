<pre><span style="white-space: normal;"><span style="font-size: medium;"><p>It's English class now. So John is bored as usual. To get over his boredom he is doing a very strange thing. He writes an arbitrary string on his notebook and then keeps changing a single character of the string every time and tries to find out &nbsp;if the string has become a palindrome.</p>
<p>As John is very smart this task is very simple for him.</p>
<p>But how simple is it for you ? Can you be as smart as the great John?</p>
<p>You'll have to write a code that solves the similar problem and hopefully as fast as John.</p>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">INPUT:</span></strong></p>
<p>First line of the input will be an integer T (T&lt;=15) denoting number of test cases.</p>
<p>Each test case starts with an integer N (1&lt;=N&lt;=100000) denoting the length of the string.</p>
<p>Next line will contain the string consisting of only small letters of English alphabet (a,b,c,...,x,y,z).</p>
<p>Then there will be another integer M (1&lt;=M&lt;=10000) denoting number of queries.</p>
<p>Each query will be in the form: &nbsp;i x</p>
<p>where i will be an integer (1&lt;=i&lt;=N) and x will be a character. (a&lt;= x&lt;=z)</p>
<p>and it will mean that the i-th character of the string has been changed to x.</p>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">OUTPUT:</span></strong></p>
<p>First you will have to print the test case number.</p>
<p>Then for each query in &nbsp;the test case you will have to print "YES" if the given string has become a plaindrome. Otherwise print &nbsp;"NO". (without the quotes )</p>
<p>See sample input/output and expalination for details.</p>
<p>&nbsp;</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="312" valign="top">
<p><strong>Sample   Input</strong></p>
</td>
<td width="312" valign="top">
<p><strong>Sample   output</strong></p>
</td>
</tr>
<tr>
<td width="312" valign="top">
<p>1</p>
<p>11</p>
<p>madamimadam</p>
<p>6</p>
<p>6 z</p>
<p>1 a</p>
<p>11 b</p>
<p>5 z</p>
<p>1 b</p>
<p>7 z</p>
<p>&nbsp;</p>
</td>
<td width="312" valign="top">
<p>Case 1:</p>
<p>YES</p>
<p>NO</p>
<p>NO</p>
<p>NO</p>
<p>NO</p>
<p>YES</p>
</td>
</tr>
</tbody>
</table>
<p><strong><span style="text-decoration: underline;">Explaination:</span></strong></p>
<p>After the 1st query the string is: madamzmadam</p>
<p>which is a palindrome</p>
<p>&nbsp;</p>
<p>After the 2nd query the string is: aadamzmadam</p>
<p>which is &nbsp;<strong>NOT</strong>&nbsp;a palindrome</p>
<p>&nbsp;</p>
<p>After the 3rd query the string is: aadamzmadab</p>
<p>which is&nbsp;<strong>&nbsp;NOT</strong>&nbsp;a palindrome</p>
<p>&nbsp;</p>
<p>After the 4th query the string is: aadazzmadab</p>
<p>which is &nbsp;<strong>NOT</strong>&nbsp;a palindrome</p>
<p>&nbsp;</p>
<p>After the 5th query the string is: badazzmadab</p>
<p>which is &nbsp;<strong>NOT</strong>&nbsp;a palindrome</p>
<p>&nbsp;</p>
<p>After the 6th query the string is: badazzzadab</p>
<p>which is a palindrome</p>
<p align="right">&nbsp;</p></span></span></pre>