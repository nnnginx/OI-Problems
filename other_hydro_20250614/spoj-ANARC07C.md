<p>&nbsp;</p>
<p>   </p>
<table style="width: 100%; background-color: #44c23c;" border="0">
<tbody>
<tr>
<td style="text-align: center;" width="50%"><a href="/problems/ANARC07C/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/ANARC07C/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Any square grid can be viewed as one or more rings, one inside the other. For example, as shown in ﬁgure (a), a 5 x 5 grid is made of three rings, numbered 1,2 and 3 (from outside to inside.) A square grid of size N is said to be sorted, if it includes the values from 1 to N^2 in a row-major order, as shown in ﬁgure (b) for N = 4. We would like to determine if a given square grid can be sorted by only rotating its rings. For example, the grid in ﬁgure (c) can<br>be sorted by rotating the ﬁrst ring two places counter-clockwise, and rotating the second ring one place in the clockwise direction.</p>
<p style="text-align: center;"><img src="../../../../../../content/simes:ANARC07C.png" alt=""></p>
<h1 style="text-align: center;">Input</h1>
<p>Your program will be tested on one or more test cases. The ﬁrst input line of a test case is an integer N which is the size of the grid. N input lines will follow, each line made of N integer values specifying the values in the grid in a row-major order. Note than 0 &lt;N ≤ 1, 000 and grid values are natural numbers less than or equal to 1,000,000.</p>
<p>The end of the test cases is identiﬁed with a dummy test case with N =0.</p>
<p>&nbsp;</p>
<p style="text-align: center;">&nbsp;</p>
<h1 style="text-align: center;">Output</h1>
<p>For each test case, output the result on a single line using the following format:</p>
<pre>k. result</pre>
<p>Where k is the test case number (starting at 1,) and result is "YES" or "NO" (without the double quotes.) and single space between "." and "result".</p>
<h1 style="text-align: center;">Sample</h1>
<pre style="text-align: justify;">input<br>4<br>9 5 1 2<br>13 7 11 3<br>14 6 10 4<br>15 16 12 8<br>3<br>1 2 3<br>5 6 7<br>8 9 4<br>0<br><br>output<br>1. YES<br>2. NO</pre>
<p> </p>