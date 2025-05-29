<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MPRIME1/en/">English</a></td>
<td width="50%"><a href="/problems/MPRIME1/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Some positive integers can be represented by a sum of one or more consecutive prime numbers.<br>How many such representations does a given positive integer have? For example, the integer 53 has two representations 5 + 7 + 11 + 13 + 17 and 53. The integer 41 has three representations 2+3+5+7+11+13, 11+13+17, and 41. The integer 3 has only one representation, which is 3. The integer 20 has no such representations. Note that summands must be consecutive prime numbers, so neither 7 + 13 nor 3 + 5 + 5 + 7 is a valid representation for the integer 20.<br><br>Your mission is to write a program that reports the number of representations for the given positive integer.</p>
<h3>Input</h3>
<p>The input is a sequence of positive integers each in a separate line. The integers are between 2 and 11 000, inclusive. The end of the input is indicated by a zero.</p>
<pre><br>SAMPLE INPUT<br>2<br>3<br>17<br>41<br>20<br>666<br>12<br>53<br>0<br></pre>
<h3>Output</h3>
<pre> <br></pre>
<p>The output should be composed of lines each corresponding to an input line except the last zero.</p>
<p>An output line includes the number of representations for the input integer as the sum of one or more consecutive prime numbers.</p>
<pre><br>SAMPLE OUTPUT<br>1<br>1<br>2<br>3<br>0<br>0<br>1<br>2<br></pre>
<p> </p>