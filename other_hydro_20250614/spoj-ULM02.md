<p><span style="font-family: 'Times New Roman'; font-size: medium;" lang="en"> </span></p>
<p><span style="font-family: arial, helvetica, sans-serif;">Consider a regular triangular area, divide it into four equal triangles of half height and remove the one in the middle. Apply the same operation recursively to each of the three remaining triangles. If we repeated this procedure infinite times, we'd obtain something with an area of zero. The fractal that evolves this way is called the Sierpinski Triangle. Although its topological dimension is&nbsp;<em>2</em>, its Hausdorff-Besicovitch dimension is<em>log(3)/log(2)~1.58</em>, a fractional value (that's why it is called a fractal). By the way, the Hausdorff-Besicovitch dimension of the Norwegian coast is approximately&nbsp;<em>1.52</em>, its topological dimension being&nbsp;<em>1</em>. </span></p>
<p style="text-align: justify;"><span style="font-family: arial, helvetica, sans-serif;">For this problem, you are to outline the Sierpinski Triangle up to a certain recursion depth, using just ASCII characters. Since the drawing resolution is thus fixed, you'll need to grow the picture appropriately. Draw the smallest triangle (that is not divided any further) with two slashes, to backslashes and two underscores like this:</span></p>
<p style="text-align: justify;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 83px; width: 1px; height: 1px; overflow: hidden;">&nbsp;/\</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 83px; width: 1px; height: 1px; overflow: hidden;">/__\</div>
<pre><span style="font-family: arial, helvetica, sans-serif;">&nbsp;/\<br></span><span style="font-family: arial, helvetica, sans-serif;">/__\</span></pre>
<p>&nbsp;</p>
<p><span style="font-family: arial, helvetica, sans-serif;"> To see how to draw larger triangles, take a look at the sample output. </span></p>
<p style="font-family: Times, serif; text-align: justify;"><strong><span style="font-family: arial, helvetica, sans-serif;">Input Specification</span></strong></p>
<p style="text-align: justify;"><span style="font-family: arial, helvetica, sans-serif;">The input contains several testcases. Each is specified by an integer&nbsp;<em>n</em>. Input is terminated by&nbsp;<em>n=0</em>. Otherwise&nbsp;<em>1��n��10</em>&nbsp;indicates the recursion depth.</span></p>
<p style="font-family: Times, serif; text-align: justify;"><strong><span style="font-family: arial, helvetica, sans-serif;">Output Specification</span></strong></p>
<p style="text-align: justify;"><span style="font-family: arial, helvetica, sans-serif;">For each test case draw an outline of the Sierpinski Triangle with a side's total length of&nbsp;<em>2<sup>n</sup></em>&nbsp;characters. Align your output to the left, that is, print the bottom leftmost slash into the first column. The output must not contain any trailing blanks. Print an empty line after each test case.</span></p>
<table style="font-family: 'Times New Roman'; margin: auto; width: 100%;" border="0" cellpadding="0">
<tbody>
<tr>
<td valign="TOP">
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Input</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>3
2
1
0
</tt></pre>
<p style="font-family: Times, serif; text-align: justify;"><strong>Sample Output</strong></p>
<p style="font-family: Times, serif; text-align: justify;"><tt></tt></p>
<pre><tt>       /\
      /__\
     /\  /\
    /__\/__\
   /\      /\
  /__\    /__\
 /\  /\  /\  /\
/__\/__\/__\/__\

   /\
  /__\
 /\  /\
/__\/__\

 /\
/__\

</tt></pre>
</td>
<td valign="BOTTOM"><img style="display: block; margin: auto;" src="file://wF68vL9w.png" alt="">
<p style="font-family: Times, serif; text-align: justify;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;The Sierpinski-Triangle up to recursion depth 7</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>