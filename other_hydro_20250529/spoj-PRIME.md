<p><span style="font-family: Verdana; font-size: x-small;"> <span style="font-size: small;">Factorial <strong>n!</strong> of an integer number <strong>n ¡Ý 0</strong> is defined  recursively as follows:<br><br></span> </span></p>
<table style="border: thin solid black;" border="0" align="center" bgcolor="#ffffff">
<tbody>
<tr>
<td><span style="font-size: small;"><strong>
<div style="margin: 15px 80px;">0! = 1 <br> n! = n * (n - 1)!</div>
</strong></span></td>
</tr>
</tbody>
</table>
<p><span style="font-size: small;"> While playing with factorials  chEEtah noticed that some of them can be represented as a product of  other         factorials, e.g. <strong>6! = 3! * 5! = 720</strong>. Such factorisation  helps chEEtah to simplify a certain class         of equations he is working on during his research. </span></p>
<p><span style="font-size: small;"> So he needs a program that finds a  compact factorisation of a given factorial or determines that it is         impossible if that is the case. If there are more than one  factorisation the program has to find such that         contains the minimum number of terms. For example, <strong>10!</strong> can be factorised in two different ways:         <strong>10! = 6! * 7! = 3! * 5! * 7!</strong>. The first factorisation  contains only two terms and should be preferred         to the second one. If there are several factorisations with the  same minimum number of terms then any optimal solution         is acceptable. </span></p>
<p><span style="font-size: small;"><span style="color: #000099; font-size: small;"><strong>Input</strong></span></span></p>
<p><span style="font-size: small;"> Input contains the only integer <strong>2 ¡Ü n  ¡Ü 1000</strong> which factorial <strong>n!</strong> should be factorised. </span></p>
<p><span style="font-size: small;"><span style="color: #000099; font-size: small;"><strong>Output</strong></span></span></p>
<p><span style="font-size: small;"> Output should contain the optimal  factorisation in the format shown in the samples. The factorisation  terms 		should go in non-decreasing order. If no factorisation can be found  print <strong>No solution</strong>. </span></p>
<h3><span style="font-size: small;">Example</span></h3>
<pre><span style="font-size: medium;"><strong>Input:</strong><br>9<br><br><strong>Output:</strong><br>9! = 2! *  3! * 3! * 7!</span><br><br></pre>