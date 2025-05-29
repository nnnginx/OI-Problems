<p>Problem</p>
<p>In A.D. 2100, aliens came to Earth.  They wrote a message in a  cryptic language, and next to it they wrote a series of symbols.  We've  come to the conclusion that the symbols indicate a number: the number of  seconds before war begins!</p>
<p>Unfortunately we have no idea what each symbol means.  We've decided  that each symbol indicates one digit, but we aren't sure what each digit  means or what base the aliens are using.  For example, if they wrote  "ab2ac999", they could have meant "31536000" in base 10 -- exactly one  year -- or they could have meant "12314555" in base 6 -- 398951 seconds,  or about four and a half days. We are sure of three things: the number  is positive; like us, the aliens will never start a number with a zero;  and they aren't using unary (base 1).</p>
<p>Your job is to determine the minimum possible number of seconds before war begins.</p>
<p>Input</p>
<p>The first line of input contains a single integer, <strong>T</strong>. <strong>T</strong> test cases follow. Each test case is a string on a line by itself. The  line will contain only characters in the 'a' to 'z' and '0' to '9'  ranges (with no spaces and no punctuation), representing the message the  aliens left us.  The test cases are independent, and can be in  different bases with the symbols meaning different things.</p>
<p>Output</p>
<p>For each test case, output a line in the following format:</p>
<pre>Case #<strong>X</strong>: <strong>V</strong></pre>
<p>Where <strong>X</strong> is the case number (starting from 1) and <strong>V</strong> is the minimum number of seconds before war begins.</p>
<p>Limits</p>
<p>1 ¡Ü <strong>T</strong> ¡Ü 100<br> The answer will never exceed 10<sup>18</sup></p>
<p>1 ¡Ü the length of each line &lt; 61</p>
<p>Sample</p>
<table style="border: 0pt solid #3127d8;" border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 3<br> 11001001<br> cats<br> zig<br> </code></td>
<td><code> Case #1: 201<br> Case #2: 75<br> Case #3: 11</code></td>
</tr>
</tbody>
</table>