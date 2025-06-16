<p>&nbsp;</p>
<h2 class="section"><span style="color: black;"> </span></h2>
<!--SEC END -->
<p>Peter is having lunch at home. Unfortunately for him, today’s meal is soup. As Peter’s mother is aware that he doesn’t like it very much, she has cooked a special soup using pasta pieces shaped like letters from the alphabet, numbers and other characters. She has a special knife with which she can prepare an unlimited supply of pasta pieces that may come in <em>S</em> different forms. The soup always has <em>P</em> pasta pieces in it, and is so thick that the pieces never move.</p>
<p>Despite her efforts, Peter is still not happy with today’s menu and asks how many days in his life he will have to eat soup. His mother promises him that she will prepare a different soup  every day, and that on no day will the dish contain the same shapes in all positions as any soup dish previously served. However, the number <em>P</em> of pasta pieces, as well as the positions in which pieces float, will remain the same every day. Peter is not easily fooled (or so he thinks), and he cleverly realizes that this can still make him eat soup for ages. In an attempt to reduce the number of configurations, he tells his mother he will not accept any dish which can be obtained by rotating one of the configurations previously seen.</p>
<blockquote class="figure">
<div class="center">
<div class="center">
<hr size="2">
</div>
<img src="../../../content/elhipercubo:dish.jpg" alt="">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">Figure 1: Top view of Peter’s dish</td>
</tr>
</tbody>
</table>
</div>
<div class="center">
<hr size="2">
</div>
</div>
</blockquote>
<p>Consider the dish as a circle of radius 2 centered at the origin. All the symbols will be floating in the soup at a given angle (in millidegrees) at distance 1 from the origin. Two plates are considered equal if you can perform a rotation of one of the dishes about its center so that the positions of the symbols, as well as the symbols themselves, are the same in both.</p>
<p>Your program will be given the number of possible symbols Peter’s mother has available, and the angles determining the location of each of the pasta pieces (measured clockwise in millidegrees). Write a program that returns the number of possible plates Peter’s mother can prepare. As this number can be very large, <strong>output the number modulo </strong><strong>100,000,007</strong>, which is prime.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of input in each test case contains two numbers: <em>S</em> (2 ≤ <em>S</em> ≤ 1,000), the number of symbols Peter’s mother can use; and <em>P</em> (<em>P</em> &gt; 0), the number of pasta pieces floating in the soup. Each of the next <em>P</em> lines contains the angle <em>A</em> (0 ≤ <em>A</em> &lt; 360,000) of one of the <em>P</em> pieces (measured clockwise in millidegrees). All angles will be different.</p>
<p>Different tests cases are separated by a blank line. After the last test case there is a line with <em>S</em> = <em>P</em> = −1.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case output a single integer in a line by itself, the number of different plates Peter’s mother can cook modulo 100,000,007.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">2 4
0
90000
180000
270000

100 5
0
45000
90000
180000
270000

-1 -1
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">6
99999307
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Javier Gómez Serrano</em></blockquote>