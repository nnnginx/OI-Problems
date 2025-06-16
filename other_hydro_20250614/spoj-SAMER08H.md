<p>It's been 100 years since the detection of the first Higgs boson and now particle physics is a mainstream subject in all high schools. Obviously, kids love the fact that they can create tiny black holes using only their portable particle accelerators and show off to their friends and colleagues. Although the creation of big black holes that could swallow the whole planet is possible even with these portable particle accelerators, the devices are programmed to only thrown particles when this undesirable side effect is impossible.</p>
<p>Your granddaughter is trying to create her own black holes with a portable accelerator kit, which is composed of two small particle accelerators that throw, each one, a boson-sized particle. Both particles are thrown at the same time, and a black hole appears when the particles collide. However, your granddaughter doesn't know how much time she'll have to wait before this happens. Fortunately, each accelerator can predict the particle's trajectory, showing four integer values into its display, called <em>A</em>, <em>B</em>, <em>C</em> and <em>D</em>. Each value can be replaced into the following equations:</p>
<table style="width: 100%;" border="0">
<tbody>
<tr>
<td>
<table border="0" cellspacing="0" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">&nbsp;</td>
<td align="center">
<table border="0">
<tbody>
<tr>
<td align="center">
<table border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td align="center"><em>r</em> = <em>At</em> + <em>B</em></td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td align="center">
<table border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td align="center">�� =  <em>Ct</em> + <em>D</em></td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</td>
<td align="center">&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>in order to determine the trajectory of the particle, in polar coordinates. The radius (r) is represented in distance units and the angle (��) in degrees. The time (t) is given in time units and it is always a rational value which can be represented by an irreducible fraction. Your granddaughter knows that in polar coordinates a point has infinite representations. In general, the point (<em>r</em>, ��) can be represented as (<em>r</em>, �� ��<em>k</em> ��360<sup><em>o</em></sup>) or ( -<em>r</em>, �� ��(2<em>k</em> + 1) ��180<sup><em>o</em></sup>), where <em>k</em> is any integer. Besides, the origin (<em>r</em> = 0) can be represented as (0, ��) for any ��.</p>
<p>Using these parameters informed by each particle accelerator, your granddaughter wants to determine whether the particles will eventually collide and, if they do, the time when they will collide. After the first collision it is impossible to predict the particle's trajectory, therefore, only the first possible collision should be considered.</p>
<p>Although your granddaughter is really intelligent and has a deep knowledge of particle physics, she does not know how to program computers and is looking for some notes in her grandfather's (or grandmother's) ICPC notebook (don't forget, she is <em>your</em> granddaughter!). Fortunately for you, there is a note on your notebook which says that you wrote that code during the 2008 ICPC South America Regional Contest (or, to be more specific, <em>this</em> contest).</p>
<h3>Input</h3>
<p>The input consists of several test cases, one per line. Each test case contains eight integer numbers separated by single spaces, <em>A</em><sub>1</sub>, <em>B</em><sub>1</sub>,<em>C</em><sub>1</sub>, <em>D</em><sub>1</sub>, <em>A</em><sub>2</sub>, <em>B</em><sub>2</sub>, <em>C</em><sub>2</sub>, <em>D</em><sub>2</sub> ( -10<sup>4</sup> �� <em>A</em><sub>1</sub>, <em>B</em><sub>1</sub>, <em>C</em><sub>1</sub>, <em>D</em><sub>1</sub>, <em>A</em><sub>2</sub>,<em>B</em><sub>2</sub>, <em>C</em><sub>2</sub>, <em>D</em><sub>2</sub> �� 10<sup>4</sup>).  The first four input values (<em>A</em><sub>1</sub>, <em>B</em><sub>1</sub>,<em>C</em><sub>1</sub>, <em>D</em><sub>1</sub>) correspond to the four parameters displayed by the first portable particle accelerator and the following input values (<em>A</em><sub>2</sub>,<em>B</em><sub>2</sub>, <em>C</em><sub>2</sub>, <em>D</em><sub>2</sub>) correspond to the four parameters displayed by the second portable particle accelerator when both particles are thrown. The end of the input is represented by <em>A</em><sub>1</sub> = <em>B</em><sub>1</sub> = <em>C</em><sub>1</sub> = <em>D</em><sub>1</sub> = <em>A</em><sub>2</sub> = <em>B</em><sub>2</sub> = <em>C</em><sub>2</sub> = <em>D</em><sub>2</sub> = 0, which should not be processed as a test case, since these are the values displayed by the particle accelerators when a big black hole would be created if the particles were trown. Although the end of input is represented by a line with eight zeroes, note that the number zero is a possible input value.</p>
<h3>Output</h3>
<p>For each test case, your program must output a line containing two non-negative integers <em>t</em><sub><em>a</em></sub> and <em>t</em><sub><em>b</em></sub> separated by a single space. If there is no possibility of collision, <em>t</em><sub><em>a</em></sub> = <em>t</em><sub><em>b</em></sub> = 0, otherwise, <em>t</em><sub><em>a</em></sub>/<em>t</em><sub><em>b</em></sub> must be an irreducible fraction representing the earliest collision time. Even if the fraction results in an integer value, you still must output the number 1 as the denominator (see samples below).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 1 180 0 2 0 180 360
10 10 360 0 -24 18 180 72
5 5 180 0 -12 9 10 40
-9 5 5 180 2 5 5 180
0 0 0 0 0 0 0 0


<strong>Output:</strong>
1 1
0 0
4 17
0 1

</pre>