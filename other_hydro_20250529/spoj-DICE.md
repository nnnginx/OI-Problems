<p>&nbsp;</p>
<div class="center"><img src="../../../content/elhipercubo:dice.jpg" alt="" width="200" height="200"></div>
<p>Just like every fall, the organizers of the Southwestern Europe Dice Simulation Contest are busy again this year. In this edition you have to simulate a 3-sided die that outputs each of three possible outcomes (which will be denoted by 1, 2 and 3) with a given probability, using three dice in a given set. The simulation is performed this way: you choose one of the given dice at random, roll it, and report its outcome. You are free to choose the probabilities of rolling each of the given dice, as long as each probability is strictly greater than zero. Before distributing the materials to the contestants, the organizers have to verify that it is actually possible to solve this task.</p>
<p>For example, in the first test case of the sample input you have to simulate a die that yields outcome 1, 2 and 3 with probabilities 3/10, 4/10 and 3/10. We give you three dice, and in this case the <em>i</em>-th of them always yields outcome <em>i</em>, for each <em>i</em> = 1, 2, 3. Then it is possible to simulate the given die in the following fashion: roll the first die with probability 3/10, the second one with probability 4/10 and the last one with probability 3/10.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of several test cases, separated by single blank lines. Each test case consists of four lines: the first three of them describe the three dice you are given and the last one describes the die you have to simulate. Each of the four lines contains 3 space-separated integers between 0 and 10&nbsp;000 inclusive. These numbers will add up to 10&nbsp;000, and represent 10&nbsp;000 times the probability that rolling the die described in that line yields outcome 1, 2 and 3, respectively.</p>
<p>The test cases will finish with a line containing only the number zero repeated three times (also preceded with a blank line).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each case, your program should output a line with the word <tt>YES</tt> if it is feasible to produce the desired die from the given ones, and <tt>NO</tt> otherwise.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">0 0 10000
0 10000 0
10000 0 0
3000 4000 3000

0 0 10000
0 10000 0
3000 4000 3000
10000 0 0

0 0 0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">YES
NO
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Abel Molina Prieto</em></blockquote>