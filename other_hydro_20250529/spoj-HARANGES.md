<p style="text-align: center;"><strong>Interesting Ranges</strong></p>
<p>A positive integer is a <em>palindrome</em> if its decimal representation (without leading zeros) is a palindromic string (a string that reads the same forwards and backwards). For example, the numbers 5, 77, 363, 4884, 11111, 12121 and 349943 are palindromes.</p>
<p>A range of integers is <em>interesting</em> if it contains an even number of palindromes. The range [L, R], with L ¡Ü R, is defined as the sequence of integers from L to R (inclusive): (L, L+1, L+2, ..., R-1, R). L and R are the range's first and last numbers.</p>
<p>The range [L<sub>1</sub>,R<sub>1</sub>] is a <em>subrange</em> of [L,R] if L ¡Ü L<sub>1</sub> ¡Ü R<sub>1</sub> ¡Ü R.  Your job is to determine how many interesting subranges of [L,R] there are.</p>
<p>Input</p>
<p>The first line of input gives the number of test cases, <strong>T</strong>.  <strong>T</strong> test cases follow. Each test case is a single line containing two positive integers, <strong>L</strong> and <strong>R</strong> (in that order), separated by a space.</p>
<p>Output</p>
<p>For each test case, output one line. That line should contain "Case #x: y", where x is the case number starting with 1, and y is the number of interesting subranges of [L,R], modulo 1000000007.</p>
<p>Limits</p>
<p>1 ¡Ü <strong>T</strong> ¡Ü 120</p>
<p>Small dataset</p>
<p>1 ¡Ü <strong>L</strong> ¡Ü <strong>R</strong> ¡Ü 10<sup>13</sup></p>
<p>Large dataset</p>
<p>1 ¡Ü <strong>L</strong> ¡Ü <strong>R</strong> ¡Ü 10<sup>100</sup></p>
<p>Sample</p>
<table style="width: 226px; height: 106px;" border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 3<br> 1 2<br> 1 7<br> 12 110<br> <br></code></td>
<td valign="top"><code> Case #1: 1<br> Case #2: 12<br> Case #3: 2466</code></td>
</tr>
</tbody>
</table>