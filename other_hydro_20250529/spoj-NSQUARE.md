<p><span style="font-family: arial, helvetica, sans-serif;"><span style="white-space: normal;"><span style="font-size: small;"> </span></span></span></p>
<p style="margin-bottom: 0in; text-align: left;">Given two integers N ( N &lt;= 10^18 ) and a prime number P ( 1 &lt; P &lt; 10^18 ), find the lowest number x  such that there're not N integers greater or equal to 0 whose sum of squares is equal to x.</p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p>&nbsp;</p>
<table style="width: 91px;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="81"> </colgroup> 
<tbody>
<tr>
<td style="border: 1px solid #000000; padding: 0.04in;" width="81" valign="TOP">
<p style="margin-bottom: 0in;" align="LEFT">N = 2, P = 2</p>
<p style="margin-bottom: 0in;" align="LEFT">x = 3mod2 = 1</p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT">0 = 0² + 0²</p>
<p style="margin-bottom: 0in;" align="LEFT">1 = 1² + 0²</p>
<p style="margin-bottom: 0in;" align="LEFT">2 = 1² + 1²</p>
<p align="LEFT">4 = 2² + 0²</p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: arial, helvetica, sans-serif;"><span style="white-space: normal;"><span style="font-size: small;"> </span></span></span></p>

<h3>Input</h3>
<p>
There're two integers N ( 1 &lt;= N &lt;= 10^18 ) and a prime number P ( 1 &lt; P &lt; 10^18 ). You have to print the answer modulo P.
</p>

<h3>Output</h3>
<p>
You have to print an integer x mod P ( -1 &lt; x &lt; 10^18 + 1 ) that satisfies the problem. If there's no number x, print "Impossible".
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1 3

<strong>Output:</strong>
2

<strong>Input:</strong>
13 7

<strong>Output:</strong>
Impossible</pre>