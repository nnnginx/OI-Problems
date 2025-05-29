<p>Year 2042. The Internet has evolved to a virtual reality dataspace where crimes are committed every day. The 2041 SWERC winner developed an agent that drops a donut every time a crime is committed in the Cyberspace. Each of the donuts has its own signature. The Madrid Police have a huge database with crimes and their donut signatures.</p>
<p>Today is your day. Your task is to implement a new agent that looks for the records in the database that bear a strong resemblance to the given signature of a dropped donut found at a new crime scene.</p>
<blockquote class="figure">
<div class="center">
<div class="center">
<hr size="2">
</div>
<img src="../../../content/elhipercubo:clue.jpg" alt="" width="250" height="150">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">Figure 1: The major piece of evidence for today’s unsolved crime streak</td>
</tr>
</tbody>
</table>
</div>
<div class="center">
<hr size="2">
</div>
</div>
</blockquote>
<p>Experts in virtual criminology have obtained the best similarity measure between donuts: compute the difference in radius of the internal part of the toroids (holes), compute the difference in radius of the external part of the toroids (tubes), and then add up those differences.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each test case contains <em>n</em> (1 ≤ <em>n</em> ≤ 50,000), the number of donuts in the database. The <em>i</em><sup><em>th</em></sup> of the following <em>n</em> lines contains the radius of the hole and radius of the tube of the <em>i</em><sup><em>th</em></sup> donut in the database, described by two integers <em>l</em> and <em>w</em> (1 ≤ <em>l</em>, <em>w</em> ≤ 10<sup>9</sup>). After that there is a line containing <em>q</em> (1 ≤ <em>q</em> ≤ 10,000), the number of donuts that you are looking for in the database. Then <em>q</em> lines follow, the <em>i</em><sup><em>th</em></sup> of them describing the dimensions of the newly found <em>i</em><sup><em>th</em></sup> donut in the same way.</p>
<p>Different test cases are separated by a blank line. A line containing −1 marks the end of the input.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>The output of your program on each test case should have <em>q</em> lines, each of them containing an integer. The <em>i</em><sup><em>th</em></sup> of these lines should contain the similarity between the newly found <em>i</em><sup><em>th</em></sup> donut and the donut in the database that most closely resembles it. Outputs for different test cases should be separated by a blank line.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">2
2 3
3 4
2
1 1
3 4

2
1 1
9 9
4
4 5
6 5
2 5
3 4

-1
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">3
0

7
7
5
5
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Abel Molina Prieto</em></blockquote>