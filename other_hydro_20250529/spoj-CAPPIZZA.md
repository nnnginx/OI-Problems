<p>Brunno Doiuna is very fond of caper pizzas, which he always likes to share with his girlfriend. As she also loves capers, it is of the utmost importance, in order to avoid unnecessary quarrels, to split the pizza into two equally-sized slices in such a way that each half contains exactly the same number of capers. However, most caper pizzas also contain a number of peppercorns, and neither Brunno nor his girlfriend likes them. Therefore, it is also crucial that each of the two halves contain the same number of peppercorns. As you can easily observe, depending on the position of capers and peppercorns on the pizza, it is not always possible to make a straight-line cut into the pizza in such a way that the two slices have the same area and the same number of capers and peppercorns lie in each resulting piece. Your task is to design a program to decide if it is possible to make such a cut or not, knowing the positions of capers and peppercorns.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Input</span></span></strong></p>
<p>We will assume that the pizza is circular and is centered at the origin, and is big enough to contain all capers and peppercorns. We also assume that there is an even number of capers and an even number of  peppercorns, and that no cut goes through any of the capers or pepper balls. Additionally, no pair of peppercorns, capers, or a peppercorn and a caper are aligned with the origin, or form an angle of less than 10<sup>−6</sup> degrees with the origin.</p>
<p>There can be multiple test cases, one after the other. The first line of a test case contains two even integers <em>c</em> ≥ 0 and <em>p</em> ≥ 0 (where 2 ≤ <em>c</em> + <em>p</em> ≤ 30000) separated by a space, the number of capers and peppercorns, respectively. Each of the following <em>c</em> lines describes the position of a caper using two floating point numbers, separated by a space, representing its <em>x</em> and <em>y</em> coordinates. Each of the next <em>p</em> lines holds two floating point numbers, the <em>x</em> and <em>y</em> coordinates of a peppercorn. A blank line follows each test case.</p>
<p>The last line of input will contain −1 −1. This marks the end of input – do not write any output for this special last line.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Output</span></span></strong></p>
<p><em>YES</em> for a positive answer, <em>NO</em> otherwise.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2 2
1 1
1 0
0 1
-1 1

2 2
1 1
-1 1
0 1
0.1 -1

-1 -1
</pre>
</div>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">NO
YES
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote">Problemsetter: Manuel Abellanas</blockquote>