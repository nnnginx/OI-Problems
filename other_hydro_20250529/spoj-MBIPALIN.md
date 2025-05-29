<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MBIPALIN/en/">English</a></td>
<td width="50%"><a href="/problems/MBIPALIN/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>&nbsp;</p>
<p>Pero and Slavko are two students who  love math. Pero  is very creative  and often comes up with new ideas. Slavko later spends days thinking  about Pero's ideas.  One day Pero and Slavko learned what a palindrome was: a string read the  same in either direction (for example,  "ANA",  "1991"  and  "RADAR"   are palindromes). Later  that day Pero  came up with  a new concept ¨C  a bipalindrome (bipalin for short).</p>
<p>A  bipalin  is  a  number,  composed  of  two  palindromes  of   the  same  length.  Both  of  these palindromes are strings of decimal digits, the first which may not start with the digit 0 (therefore, the  entire bipalin may not start with a 0). For example, 393020 is a  bipalin (composed of the palindromes 393 and 020), while 222 and 010202  are not.</p>
<p>After hearing about bipalins, Slavko started thinking. After half an  hour he found that there is only one bipalin of length 6 that is divisible by 12345. This is the bipalin 555525. Shocked by this finding, he wants  you to write a program that, given two integers N and M, calculates the  number of different bipalins of length N that are divisible by M.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>Input consists of two integers N and M (2 ¡Ü N ¡Ü 20, 1 ¡Ü M ¡Ü 1 000 000),  where N is even.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>Output the number of different bipalins of length N that are divisible by M.</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>input 
6 123 
output 
71 

input 
2 10 
output 
9

input 
6 12345 
output 
1 
</pre>
<p> </p>