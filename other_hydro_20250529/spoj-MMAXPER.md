<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MMAXPER/en/">English</a></td>
<td width="50%"><a href="/problems/MMAXPER/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given  are n  rectangles,  numbered  from 1 to n. We place  them tightly on  the  axis OX,  from  left  to right, according to rectangles' numbers. Each rectangle stays on the axis OX either by its shorter or by its longer side (see the picture below). Compute the  length of the upper envelop line, i.e. perimeter's length of the obtained figure minus  the  length of  the  left, right and bottom straight line segments of the picture. Write program to find the maximum possible length of the upper envelop line.</p>
<p><img src="../../../content/simes:MMAXPER.png" border="0" alt=""></p>
<h3>Input</h3>
<p>On  the  first  line  of  the  standard  input,  the  value  of  n is written. On  each  of  the  next  n  lines,  two integers are given ¨C a_i  and b_i ¨C the side lengths of the i_th rectangle.</p>
<p>Constraints:  0 &lt; n &lt; 1000; 0 &lt; a_i &lt; b_i &lt; 1000, for each i = 1, 2, ¡­, n.</p>
<h3>Output</h3>
<p>On a line of the standard output, your program should write the result as a positive integer.</p>
<pre><strong>SAMPLE INPUT:</strong>
5
2 5
3 8
1 10
7 14
2 5
</pre>
<pre><strong>SAMPLE OUTPUT:</strong>
68
</pre>
<h3>Explanation</h3>
<p>A configuration, that yields the maximum length of the upper envelopline, is presented on the picture. The  upper  envelop  line  consists  of  segments DC, CG, GF, FJ,  JI,  IM, ML, LP,  and PO. The  total length is 5 + 6 + 3 + 7 + 10 + 13 + 7 + 12 + 5 = 68</p>
<p><strong>Problem for kid - Please, think like kid.</strong>  </p>