<p>After a long week of work at the ICPC Headquarters, Bill and his friends usually go to a small pub on Friday evenings to have a couple of beers and play darts. All of them are well aware of the fact that their ability at darts decreases at the same rate as the amount of beer left in their mugs.</p>
<p>They always play 501, one of the easiest games. Players start with a score of <em>N</em> points (typically, <em>N</em>=501, hence the name) and take turns throwing darts. The score of each player decreases by the value of the section hit by the dart, unless the score becomes negative, in which case it remains unchanged. The first player to reach a score of 0 wins. The figure below shows the dartboard with which the game is played.</p>
<blockquote class="figure">
<div class="center"><img src="../../../content/elhipercubo:dartboard.jpg" alt="" width="250" height="250">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">Dartboard</td>
</tr>
</tbody>
</table>
</div>
</div>
</blockquote>
<p>As the clock ticks closer to midnight and they start running out of beer, everyone wonders the same: is it worth trying to aim the dart at a specific section? Or is it better just to throw the dart at a random section on the dartboard? You are asked to deal with the question by finding out what would happen if two players (A and B) applying these two different strategies were to play against each other:</p>
<ul class="itemize">
<li class="li-itemize">Player A throws the darts at random, and consequently they land with equal probability in each of the sections of the dartboard.</li>
<li class="li-itemize">If Player B aims at a certain section, the dart has the same probability of landing in the correct one as in each of the two adjacent ones (the neighbouring regions to the left and right). Moreover, he is completely aware of his ability and sober enough to aim at the section that maximizes his probability of winning.</li>
</ul>
<p>Given the initial score of both players, can you determine the probability that the first player wins? Of course, being the first to throw a dart might be advantageous, so the answer depends on who plays first.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of a series of lines, each containing an integer <em>N</em> (1 ≤ <em>N</em> ≤ 501), the initial score of both players. A case with <em>N</em> = 0 marks the end of the input and must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each number in the input, your program should output a line containing two real numbers: the probability that <em>A</em> wins if <em>A</em> throws the first dart, and the probability that <em>B</em> wins if <em>B</em> throws the first dart. Your answers should be accurate to within an absolute or relative error of 10<sup>−8</sup>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">5
100
0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">0.136363636364 0.909090909091
0.072504908290 0.950215081962
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Luis Hernández Corbato</em><em>&nbsp;</em></blockquote>