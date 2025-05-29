<p>Computing the number of fixed points and, more generally, the number of periodic orbits within a dynamical system is a question attracting interest from different fields of research. However, dynamics may turn out to be very complicated to describe, even in seemingly simple models. In this task you will be asked to compute the number of periodic points of period <em>n</em> of a piecewise linear map <em>f</em> mapping the real interval [0,<em>m</em>] into itself. That is to say, given a map <em>f</em> : [0, <em>m</em>] → [0, <em>m</em>] you have to calculate the number of solutions to the equation <em>f</em><sup><em>n</em></sup>(<em>x</em>) = <em>x</em> for <em>x</em> ∈ [0, <em>m</em>], where <em>f</em><sup><em>n</em></sup> is the result of iterating function <em>f</em> a total of <em>n</em> times, i.e.</p>
<table class="display dcenter" border="0">
<tbody>
<tr valign="middle">
<td class="dcell"><em>f</em><sup><em>n</em></sup>&nbsp;=&nbsp;</td>
<td class="dcell">
<table class="display" border="0">
<tbody>
<tr>
<td class="dcell" align="center"><em>n</em>&nbsp;<em>f</em>′<em>s</em></td>
</tr>
<tr>
<td class="dcell" align="center">
<table class="display" style="width: 100%;" border="0">
<tbody>
<tr>
<td class="dcell" style="width: 5%;" align="center">◢</td>
<td class="dcell" style="width: 40%;" align="center">
<hr class="hbar">
</td>
<td class="dcell" style="width: 10%;" align="center"></td>
<td class="dcell" style="width: 40%;" align="center">
<hr class="hbar">
</td>
<td class="dcell" style="width: 5%;" align="center">◣</td>
</tr>
<tr>
<td class="dcell" colspan="5" align="center"><em>f</em>&nbsp;∘&nbsp;..&nbsp;∘&nbsp;<em>f</em>&nbsp;∘&nbsp;<em>f</em></td>
</tr>
<tr>
<td class="dcell" colspan="5" align="center">&nbsp;</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="dcell" align="center">&nbsp;</td>
</tr>
</tbody>
</table>
</td>
<td class="dcell">,</td>
</tr>
</tbody>
</table>
<p>where ∘ stands for the composition of maps, (<em>g</em> ∘ <em>h</em>) (<em>x</em>) = <em>g</em>(<em>h</em>(<em>x</em>)).</p>
<p>Fortunately, the maps you will have to work with satisfy some particular properties:</p>
<ul class="itemize">
<li class="li-itemize"> <em>m</em> will be a positive integer and the image of every integer in [0,<em>m</em>] under <em>f</em> is again an integer in [0,<em>m</em>], that is, for every <em>k</em> ∈ {0, 1, … , <em>m</em>} we have that <em>f</em>(<em>k</em>) ∈ {0, 1, … , <em>m</em>}.</li>
<li class="li-itemize">For every <em>k</em> ∈ {0, 1, …, <em>m</em> − 1}, the map <em>f</em> is linear in the interval [<em>k</em>, <em>k</em> + 1]. This means that for every <em>x</em> ∈ [<em>k</em>, <em>k</em> + 1], its image satisfies <em>f</em>(<em>x</em>) = (<em>k</em> + 1 − <em>x</em>)<em>f</em>(<em>k</em>) + (<em>x</em> − <em>k</em>)<em>f</em>(<em>k</em> + 1), which is equivalent to its graph on [<em>k</em>,<em>k</em> + 1] being a straight line segment. </li>
</ul>
<blockquote class="figure">
<div class="center">
<div class="center">
<hr size="2">
</div>
<img src="../../../content/elhipercubo:mapexample.jpg" alt=""> &nbsp;&nbsp;&nbsp;&nbsp; <img src="../../../content/elhipercubo:mapexample2.jpg" alt="">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">Figure 1: Graphs of the third map in the sample input, <em>f</em><sub>3</sub> (left), and of its square, <em>f</em><sub>3</sub><sup>2</sup> (right).</td>
</tr>
</tbody>
</table>
</div>
<div class="center">
<hr size="2">
</div>
</div>
</blockquote>
<p>Since there might be many periodic points you will have to output the result modulo an integer.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Input</span></span></strong></p>
<p>The input consists of several test cases, separated by single blank lines. Each test case begins with a line containing the integer <em>m</em> (1 ≤ <em>m</em> ≤ 80). The following line describes the map <em>f</em>; it contains the <em>m</em> + 1 integers <em>f</em>(0), <em>f</em>(1), …, <em>f</em>(<em>m</em>), each of them between 0 and <em>m</em> inclusive. The test case ends with a line containing two integers separated by a blank space, <em>n</em> (1 ≤ <em>n</em> ≤ 5&nbsp;000) and the modulus used to compute the result, <em>mod</em> (2 ≤ <em>mod</em> ≤ 10&nbsp;000).</p>
<p>The input will finish with a line containing <tt>0</tt>.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Output</span></span></strong></p>
<p>For each case, your program should output the number of solutions to the equation <em>f</em><sup><em>n</em></sup>(<em>x</em>) = <em>x</em> in the interval [0, <em>m</em>] modulo <em>mod</em>. If there are infinitely many solutions, print <tt>Infinity</tt> instead.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2
2 0 2
2 10

3
0 1 3 2
1 137

3
2 3 0 3
20 10000

0
</pre>
</div>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">4
Infinity
9074
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em> Problemsetter: Luis Hernández Corbato </em></blockquote>