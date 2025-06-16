<p>Let's call a matrix <em>A[3 x 3]</em> Dinostratus if all its nine elements are different positive integer numbers and each its element <em>a<sub>i,j</sub></em> (where 1 ¡Ü <em>i</em>,<em>j</em> ¡Ü 3) is a multiple of  its neighbors <em>a<sub>i-1,j</sub></em>, <em>a<sub>i-1,j-1</sub></em> and <em>a<sub>i,j-1</sub></em> (if they exist). In other words the following conditions hold:</p>
<ul>
<li><em>a<sub>i,j</sub></em> = <em>X</em> ¡¤ <em>a<sub>i-1,j</sub></em> for some positive integer <em>X</em> (if <em>i</em>&nbsp;¡Ý 2)</li>
<li><em>a<sub>i,j</sub></em> = <em>Y</em> ¡¤ <em>a<sub>i,j-1</sub></em> for some positive integer <em>Y</em> (if <em>j</em> ¡Ý 2)</li>
<li><em>a<sub>i,j</sub></em> = <em>Z</em> ¡¤ <em>a<sub>i-1,j-1</sub></em> for some positive integer <em>Z</em> (if <em>i</em>,<em>j</em> ¡Ý 2)</li>
</ul>
<p>For example the matrices</p>
<table border="0" align="center">
<tbody>
<tr>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">1&nbsp;</td>
<td style="width: 30px;" align="right">3&nbsp;</td>
<td style="width: 30px;" align="right">9&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;2&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;6&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;18&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;4&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;12&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;36&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
<td>&nbsp;&nbsp;&nbsp;</td>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">3&nbsp;</td>
<td style="width: 30px;" align="right">18&nbsp;</td>
<td style="width: 30px;" align="right">198&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;21&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;126&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;4158&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;147&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;882&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;29106&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
<td>&nbsp;&nbsp;&nbsp;</td>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">10&nbsp;</td>
<td style="width: 30px;" align="right">100&nbsp;</td>
<td style="width: 30px;" align="right">4000&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;50&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;1000&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;20000&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;10000&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;100000&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;1000000&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>are Dinostratus. And the following matrices are not:</p>
<table border="0" align="center">
<tbody>
<tr>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">1&nbsp;</td>
<td style="width: 30px;" align="right">3&nbsp;<br></td>
<td style="width: 30px;" align="right">9&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;2&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;6&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;18&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;4&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;12&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;54&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
<td>&nbsp;&nbsp;&nbsp;</td>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">1&nbsp;</td>
<td style="width: 30px;" align="right">2&nbsp;</td>
<td style="width: 30px;" align="right">4&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;2&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;4&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;8&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;4&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;8&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;16&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
<td>&nbsp;&nbsp;&nbsp;</td>
<td>
<table border="2">
<tbody>
<tr>
<td>
<table border="0" cellspacing="2" cellpadding="2">
<tbody>
<tr>
<td style="width: 30px;" align="right">36&nbsp;</td>
<td style="width: 30px;" align="right">12&nbsp;</td>
<td style="width: 30px;" align="right">4&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;18&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;6&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;2&nbsp;</td>
</tr>
<tr>
<td style="width: 30px;" align="right">&nbsp;9&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;3&nbsp;</td>
<td style="width: 30px;" align="right">&nbsp;1&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>Let's define the element <em>a<sub>3,3</sub></em> of a Dinostratus matrix <em>A[3 x 3]</em> as a <strong>base number</strong>. Given a base number, find out how many different Dinostratus matices exist. Two matrices <em>A</em> and <em>B</em> are different if there are such indexes <em>i</em>, <em>j</em> that <em>a<sub>i,j</sub></em> ¡Ù <em>b<sub>i,j</sub></em>.</p>
<h3>Input</h3>
<p>Input file consists of several test cases. Input file starts with a line containing an integer <em>T</em> (<em>T</em> ¡Ü 500), which is the number of test cases. The next <em>T</em> lines constain one base number <em>N</em> (1 ¡Ü <em>N</em>&nbsp;¡Ü 1000000).</p>
<h3>Output</h3>
<p>For each test case output a single line containing the number of different Dinostratus matrices corresponding to the base number. It is guaranteed that the answer is less than 2<sup>63</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7<br>1<br>10<br>100<br>1000<br>10000<br>100000<br>1000000

<strong>Output:</strong>
0<br>0<br>2<br>2382<br>257110<br>7475718<br>106889830
</pre>
<h3>Note</h3>
<p>You can try the problem <a href="../../problems/DINONUM">DINONUM</a> first.</p>