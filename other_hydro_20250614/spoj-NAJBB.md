<p>Boss Baby is the boss of all babies. He has been exploring prime numbers lately, and new recently made a conjecture resembling one of Goldbach's conjectures. Boss baby¡¯s conjecture is that any number greater than or equal 10 can be expressed as the sum of a prime, square of two prime. It¡¯s very easy work for him but he is busy to stop the dastardly plot of the CEO of Puppy Co. &nbsp;He wants your help verify his conjecture for small numbers.</p>
<p>Note: 1 is not a prime number.</p>
<p><strong>Input:</strong></p>
<p>The first line of the input contains an integer T(T¡Ü10^6) denoting the number of test cases. Each test case contain Input will consist of a series of numbers greater than 10 and less than 10^6, one per line</p>
<p><strong>Output:</strong></p>
<p>For each case, print the case number and print 3 primes P<sub>1</sub>, P<sub>2</sub>, P<sub>3</sub> on a line, where P<sub>1</sub> + P<sub>2</sub><sup>2</sup> + P<sub>3</sub><sup>2</sup> is equal to the number from the input. (P1, P2, P3 must be print in sort order) If no such primes exist, print "0 0 0" instead (quotes for clarity). If there are multiple triplets of primes that satisfy the equation, print the least one in softed order.</p>
<p><strong>Sample:</strong></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="258" valign="top">
<p>Input</p>
</td>
<td width="198" valign="top">
<p>Output</p>
</td>
</tr>
<tr>
<td width="258">
<p>3<br>18<br>20<br>23</p>
</td>
<td width="198">
<p>Case   1: 2 3 5<br>Case   2: 2 3 3<br>Case   3: 3 3 5</p>
</td>
</tr>
</tbody>
</table>
<p><strong>&nbsp; <br></strong></p>
<p>Note:</p>
<p>For second Case 20<br>2,3,3(2+3<sup>2</sup>+3<sup>2</sup>) =20 and &nbsp;2,3,7 (2<sup>2</sup>+3<sup>2</sup>+7)=20 is possible<br>but 2,3,3 is the least one</p>