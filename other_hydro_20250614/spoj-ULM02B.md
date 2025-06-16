<p><span style="font-family: 'Times New Roman'; font-size: 16px;">Computer scientists live on pizza. Now the doctors say this is no good. We ought to eat more balanced. So you put your really large pizza onto your table and eat slice-by-slice carefully watching that the rest of your meal stays where it is - on the table.</span></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Since computer scientists love pizza, their favourite table is shaped like a slice of pizza. However, different people may have different-sized tables. Everyone has his own preference for the number of slices a pizza has to be cut to. However, all agree that the slices must have identical size. Write a program to help the poor pizza lovers!</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Input Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">The input file contains several test cases. Each test case starts with the number of slices&nbsp;<em>n</em>&nbsp;the pizza is cut to. Input is terminated by&nbsp;<em>n=0</em>. Otherwise,&nbsp;<em>1��n��9</em>. Then follow 9 floating-point numbers&nbsp;<em>p<sub>x</sub>, p<sub>y</sub>, r, t<sub>x</sub>, t<sub>y</sub>, u<sub>x</sub>, u<sub>y</sub>, v<sub>x</sub>, v<sub>y</sub></em>&nbsp;specifying the coordinates of the center&nbsp;<em>p</em>&nbsp;of the pizza, its radius, and the coordinates of three points&nbsp;<em>t, u, v</em>. They define the three corners of the slice-shaped table in counter-clockwise order, with&nbsp;<em>t</em>being the center.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">The pizza is a homogeneous two-dimensional circular object. There is always a cut from its center parallel to the x-axis towards increasing x-values. The remaining pizza stays connected during the whole process, no matter what slices are removed. The distances from&nbsp;<em>t</em>&nbsp;to&nbsp;<em>u, v</em>&nbsp;are equal except for very small rounding errors. Tables are never larger than a half-circle.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Output Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">For each test case output on a line some possible ordering of slices, so that during the whole process of eating the pizza it does not fall down the table. Slices are numbered counter-clockwise starting with 1 directly above the positive x-axis.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">If several such ordering exist, choose the lexicographically first one.&nbsp;<br>If no ordering of slices exists, so that the pizza does not fall down, output a line containing the word "impossible" instead.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Remark</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">A connected, rigid, flat object remains fixed on a convex, flat surface if and only if the object's center of gravity lies above the surface. The x-coordinate, for example, of the center of gravity of an object&nbsp;<em>s</em>&nbsp;can be calculated by (��<sub><em>s</em></sub><em>x</em>d<em>s</em>) / (��<sub><em>s</em></sub>d<em>s</em>). Likewise, the y-coordinate can be expressed as (��<sub><em>s</em></sub><em>y</em>d<em>s</em>) / (��<sub><em>s</em></sub>d<em>s</em>). Note that the denominator of these expressions gives the area of&nbsp;<em>s</em>.</p>
<table style="margin: auto; width: 100%;" border="0" cellpadding="0">
<tbody>
<tr>
<td valign="TOP">
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Input</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>2 (-3.0,-1.0) 1.0 (-3.0,-1.1) (-1.5,0.4) (-4.5,0.4)
9 (2.0,1.0) 1.0 (0.0,0.0) (1.0,-1.0) (-1.0,1.0)
0
</tt></pre>
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Output</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>2 1
impossible
</tt></pre>
</td>
<td valign="TOP"><img style="display: block; margin: auto;" src="file://rBLKZIoD.png" alt=""></td>
</tr>
</tbody>
</table>