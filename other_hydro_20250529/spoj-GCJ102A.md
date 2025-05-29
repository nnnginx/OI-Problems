<h3>Problem</h3>
<p>The king has hired you to make him an elegant diamond.  An elegant  diamond is a two-dimensional object made out of digits that's symmetric  about a horizontal and a vertical axis.  For example, the following four  shapes are elegant diamonds:</p>
<pre>   2       8      3     7
  3 3     8 8    2 2
 4 1 4     8      3
  3 3 
   2
</pre>
<p>These three shapes are diamonds, but are not elegant:</p>
<pre>  2       1        3
 1 1     1 2      1 1
  1     1 1 1    3 1 3
         2 1      1 1
          1        2
</pre>
<p>These three shapes are not diamonds:</p>
<pre>  1     2     8   8
 1 1   222      0
        2     00000
</pre>
<p>The king will start by giving you a diamond, which may not be elegant.  Your job is to make it elegant by  <em>enhancing</em> it, adding digits on to make a bigger diamond.  Because you don't want  to spend too much money, you want to do it with as little <em>cost</em> as possible.</p>
<h3>Definitions</h3>
<p>A <strong>diamond of size <em>k</em></strong> is 2k-1 lines of digits, 0-9, separated by single spaces, organized in the following way:</p>
<ul>
<li>Line i (1 �� i �� k) contains k-i spaces, then i digits separated by single spaces.</li>
<li>Line i (k &lt; i &lt; 2k) contains i-k spaces, then 2k-i digits separated by single spaces.</li>
</ul>
<p>An <strong>elegant diamond of size <em>k</em></strong> is a diamond of size k with the following two symmetry properties:</p>
<ul>
<li>Horizontal symmetry: Let c<sub>i</sub> be the number of digits on line i.  The j<sup>th</sup> digit on line i (where j=1 for the first digit) must be the same as the c<sub>i</sub>+1-j<sup>th</sup> digit.</li>
<li>Vertical symmetry: The j<sup>th</sup> digit on line i (where i=1 for the first line) must be the same as the j<sup>th</sup> digit on line 2k-i.</li>
</ul>
<p>A diamond of size k can be <strong>enhanced</strong> by adding digits to it.  The result of enhancing a diamond of size k has the following properties:</p>
<ul>
<li>The result is a diamond of size �� k.</li>
<li>The original diamond is part of the result. In other words, there  exist some X and some Y such that, for all values of i and j such that  the j<sup>th</sup> character of the i<sup>th</sup> line of the original is a digit (as opposed to a space), the j+X<sup>th</sup> character on the i+Y<sup>th</sup> line of the result is also a digit and it's the same as the j<sup>th</sup> character on the i<sup>th</sup> line of the original. </li>
</ul>
<p>The <strong>cost</strong> of enhancing a diamond is equal to the number of digits  in the result of the enhancement, minus the number of digits in the  original diamond.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases, <strong>T</strong>.  <strong>T</strong> test cases follow.  Each test case consists of a single integer <strong>k</strong> in a line on its own, followed by a diamond of size <strong>k</strong>.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is  the case number (starting from 1) and y is the minimum cost required to  enhance the given diamond into an elegant diamond.  If the diamond is  already elegant, y=0.</p>
<h3>Limits</h3>
<p>1 �� <strong>T</strong> �� 100.</p>
<h4>Large dataset</h4>
<p>1 �� <strong>k</strong> �� 51.</p>
<h3>Sample</h3>
<div>
<table border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 4<br> 1<br> 0<br> 2<br> &nbsp;1<br> 2 2<br> &nbsp;1<br> 2<br> &nbsp;1<br> 1 2<br> &nbsp;1<br> 3<br> &nbsp;&nbsp;1<br> &nbsp;6 3<br> 9 5 5<br> &nbsp;6 3<br> &nbsp;&nbsp;1<br> </code></td>
<td><code> Case #1: 0<br> Case #2: 0<br> Case #3: 5<br> Case #4: 7<br> <br> </code></td>
</tr>
</tbody>
</table>
</div>
<h3>Explanation</h3>
<p>There are four cases.  The first two cases start as elegant diamonds of  size 1 and 2, respectively, and don't need to be enhanced; so the cost  is 0.  The third case can be enhanced to look like:</p>
<pre>  3
 1 1
1 2 1
 1 1
  3
</pre>
<p>There are several possible enhancements, but this is one with the lowest  possible cost, which is 5.  In the fourth case we can enhance the  diamond into the following elegant diamond:</p>
<pre>   9
  1 1
 6 3 6
9 5 5 9
 6 3 6
  1 1
   9
</pre>
<p>...for a cost of 7.</p>