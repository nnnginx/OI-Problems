<p>Scientist Aftab has made a groundbreaking discovery regarding chromosomal crossover today!<br> <br> Before going into details let¡¯s understand a few definitions first. According to Holland¡¯s convention, a gene is represented by either 0 or 1. A chromosome is a string of genes. While in crossover, two parental chromosomes arbitrarily get separated at the exact same position forming four non-empty parts. &nbsp;And these parts join together to form two offspring. For example, let A and B be two parental chromosomes of length N. After cutting those at arbitrary position X, we get four parts LA, RA, LB, RB. Here LA is made of A[0,¡­,X], RA is made of A[X+1,¡­,N-1] and the same for LB and RB. After applying crossover, we get two offspring O1=LA+RB andO2= LB+RA. Here ¡®+¡¯ is string concatenation operator.</p>
<p>Scientist Aftab¡¯s claim is that, the fittest offspring among O1 and O2 is the one which is greater in value. Here the value of a chromosome is computed keeping in mind that this is a bitstring with the leftmost bit being the Most Significant Bit (MSB) and the rightmost bit is the Least Significant Bit (LSB).</p>
<p>Although scientist Aftab is a great genetics researcher, he is not good at handling chromosomes of large size. So he is seeking your help. You will be given two chromosomes of length N. And you will have to output the decimal value modulo 10<sup>9</sup>+7 of the fittest offspring after applying crossover.</p>
<h3>Input</h3>
<p>Input starts with an integer <strong>T(&lt;=30)</strong>, denoting the number of test cases. Each case contains two lines containing two strings of same length <strong>N (2&lt;=N&lt;=100000)</strong>. Strings will contain only 0¡¯s and 1¡¯s.</p>
<h3>Output</h3>
<p>For each case of input, print the case number followed by the decimal value modulo 10<sup>9</sup>+7 of the fittest string after the crossover.</p>
<h3>Sample I/O</h3>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="308" valign="top">
<p>Input</p>
</td>
<td width="308" valign="top">
<p>Output</p>
</td>
</tr>
<tr>
<td width="308" valign="top">
<p>2</p>
<p>100101</p>
<p>110010</p>
<p>10010</p>
<p>11101</p>
</td>
<td width="308" valign="top">
<p>Case 1: 53</p>
<p>Case 2: 30</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<h3>Explanation of Sample I/O</h3>
<p>For the first case, the fittest offspring is 110101, whose decimal value modulo 10<sup>9</sup>+7 is 53.</p>