<!-- 		@page { margin: 0.79in } 		td p { margin-bottom: 0in } 		pre.cjk { font-family: "Nimbus Mono L", monospace } 		p { margin-bottom: 0.1in; line-height: 120% } 	 -->
<pre style="page-break-before: always;"><p>One day little girl Lilith was playing with strings. She made a string X which is a palindrome! Suddenly her favorite dog </p><p>¡°hehway¡± came and ate some of the characters from X but not all! Lilith built another palindrome but naughty ¡°hehway¡± </p><p>came again and destroyed it! Watching this happening again and again Lilith¡¯s boyfriend Mada thought that he can give her </p><p>a machine as birthday present that automatically converts any string to palindrome by adding some characters. The machine </p><p>will be connected with an infinite supply of lowercase Latin characters(¡®a¡¯-¡¯z¡¯).</p><p>&nbsp;</p><p>The machine also has two amazing features :</p><p>1. The machine always adds minimum number of characters to the input string in order to&nbsp; convert it to a palindrome.</p><p>2. If there are multiple ways then it always produces the lexicographically smallest palindrome.</p><p>&nbsp;</p><p>We all know that machines are not perfect! So, there is no way to guaranty that the machine generated palindrome is the </p><p>original palindrome that Lilith made in the first place! But, ¡°Mada¡± thought that it will at least help Lilith to forget the</p><p>sorrow of losing her favorite palindromes to her favorite dog!&nbsp;</p><p>So, when you enter a string X into the machine, the machine¡¯s output looks like N Y, where N is number of new characters </p><p>that it added to X to make Y. And Y is the lexicographically minimum palindrome produced by adding 0 or more characters </p><p>with X.</p><p>Can you help ¡°Mada¡± with the algorithm of the machine?</p><p>&nbsp;</p><p><strong>Input :</strong></p><p>The first line of input determines the number of test cases (1&lt;=T&lt;=2000). Each of the next T lines contains a </p><p>string S (1&lt;=|s|&lt;=100). S is a string which is left after Lilith¡¯s dog ¡°hehway¡± ate </p><p>some of the characters(possibly none!) of the original string. S will be the input of the machine.</p><p><strong>Output : </strong></p><p>Print the machine¡¯s output in each line along with the case number!&nbsp; See Sample test cases for I/O format and </p><p>explanation for more clarification about the problem.</p><p>&nbsp;</p><span style="font-size: small;"><span style="white-space: normal;"><table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p align="center"><strong>Sample Input</strong></p>
</td>
<td width="319" valign="top">
<p align="center"><strong>Sample Output</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p>4</p>
<p>ab</p>
<p>aba</p>
<p>abcd</p>
<p>bca</p>
<p>&nbsp;</p>
</td>
<td width="319" valign="top">
<p>Case 1:   1 aba</p>
<p>Case 2:   0 aba</p>
<p>Case 3:   3 abcdcba</p>
<p>Case 4: 2 abcba</p></td></tr></tbody></table></span></span><p>&nbsp;</p><p><br><strong>Explanation :</strong></p><p>First input ¡°ab¡± =&gt; We can add a ¡®b¡¯ to its beginning which will make it ¡°bab¡± we can also add an ¡®a¡¯ to its end which till </p><p>make it ¡°aba¡±. In either way we are adding one extra character but ¡°aba¡± is lexicographically smaller than ¡°bab¡±. So our</p><p>result is ¡°aba¡±. We can also add ¡°ba¡± to the end of ¡°ab¡± which will result into ¡°abba¡± which is also a palindrome, but in </p><p>that case we would need two characters instead of one. We need to ensure minimal character insertion at first and then</p><p>try to minimize the result lexicographically. </p><p>See this way, (a) + ab + (ba + a) results into ¡°aabbaa¡± which is lexicographically smaller than ¡°aba¡± but it needs 4 </p><p>characters to build that palindrome where ¡°aba¡± needs only 1. So, ¡°aba¡± is the desired result!</p><p>&nbsp;</p><p><strong>In second case the string is already a palindrome!&nbsp; </strong></p><p><strong>Look at the fourth case. We are allowed to add character at any position of the given string not only just </strong></p><p><strong>at beginning or end!</strong></p></pre>