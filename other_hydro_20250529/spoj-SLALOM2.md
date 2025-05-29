<div class="center"><img src="../../../content/elhipercubo:slalom.jpg" alt="" width="300" height="400"></div>
<p>In spite of the scarcity of snowfall in Madrid, interest in winter sports is growing in the city, especially with regard to skiing. Many people spend several weekends or even full weeks improving their skills in the mountains.</p>
<p>In this problem we deal with only one of the multiple alpine skiing disciplines: slalom. A course is constructed by laying out a series of gates, which are formed by two poles. The skier must pass between the two poles forming each gate. The winner is the skier who takes the least time to complete the course while not missing any of the gates.</p>
<p>You have recently started to learn to ski, but you have already set yourself the goal of taking part in the Winter Olympic Games of 2018, for which Madrid will presumably present a candidature. As part of the theoretical training, you need to write a program that calculates, given a starting point and a series of gates, the minimum-length path starting from the point given and passing through each gate until you reach the last one, which is the finish line. You may assume that the gates are horizontal and are ordered from highest to lowest, so that you need to pass through them in order. You consider yourself an accomplished skier, so you can make any series of turns, no matter how difficult, and your only concern is minimizing the total length of the path.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each case gives the number of gates <em>n</em> (1 ≤ <em>n</em> ≤ 1&nbsp;000). The next line contains two floating point numbers, the Cartesian coordinates <em>x</em> and <em>y</em> of the starting position, in that order. Next come <em>n</em> lines with three floating point numbers each, <em>y</em>&nbsp;<em>x</em><sub>1</sub>&nbsp;<em>x</em><sub>2</sub>, meaning that the next gate is a horizontal line from (<em>x</em><sub>1</sub>, <em>y</em>) to (<em>x</em><sub>2</sub>, <em>y</em>). You can safely assume that <em>x</em><sub>1</sub> &lt; <em>x</em><sub>2</sub>. The values of <em>y</em> are strictly decreasing and are always smaller than that of the starting position. The last gate represents the finish line. All coordinates are between −500&nbsp;000 and 500&nbsp;000, inclusive. A value of 0 for <em>n</em> means the end of the input. A blank line follows each case.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, output a line with the minimum distance needed to reach the finish line. Your answer should be accurate to within an absolute or relative error of 10<sup>−7</sup>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2
0 2
1 1 2
0 0.5 3

3
0 4
3 1 2
2 -1 0
1 1 2

0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2.41421356237
4.24264068712
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Manuel Abellanas</em></blockquote>