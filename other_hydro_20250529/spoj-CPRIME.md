<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/CPRIME/en/">English</a></td>
<td width="50%"><a href="/problems/CPRIME/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>In number theory, the Prime Number Theorem describes the asymptotic distribution of prime numbers. Let ¦Ð(x) be the number of prime numbers not greater than x. The Prime Number Theorem states that:</p>
<p><img src="file://0re9JeNK.png" alt=""></p>
<p>Your task is to write a program to verify how well the Prime Number Theorem can estimate ¦Ð(x). To be more precise, for a given x, you have to calculate the percent error |¦Ð(x) - x/lnx| / ¦Ð(x) %.</p>
<h3>Input</h3>
<p>The input contains several test cases (no more than 1000). Each test case contains a value of x (2 ¡Ü x ¡Ü 10<sup>8</sup>) given in one line. A number 0 terminates the input.</p>
<h3>Output</h3>
<p>For each value of x, output the percent error of the estimation of ¦Ð(x), rounded to 1 decimal digit.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10000000
2
3
5
1234567
0

<strong>Output:</strong>
6.6
188.5
36.5
3.6
7.7
</pre>
<p> </p>