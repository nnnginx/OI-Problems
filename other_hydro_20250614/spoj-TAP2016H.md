<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>We are considering changing the rules for the Argentinian Programming Tournament starting next year. Before doing that, we would like to evaluate whether the new system is fair, and we need your help to do that.</p>
<p>The new tournament will have <strong>N</strong>&nbsp;teams competing in <strong>N-1</strong>&nbsp;rounds. In each round two teams will face each other competing in order to be the first to solve a problem, the losing team being eliminated. In the first round, two teams will be chosen at random, and the losing team will be placed in the last place of the scoreboard, while the winner remains in the competition. In each of the following rounds, two teams still in the competition will be chosen at random, and the losing team shall be placed in the last remaining place of the scoreboard, being thus eliminated from the tournament.</p>
<p>For example, if the tournament has <strong>N=4</strong>&nbsp;teams named "<em>aWArush</em>", "<em>Buen Kilo de Pan Flauta</em>", "<em>Melarita</em>"&nbsp;and "<em>Type Mismatch</em>", the tournament will be held in three rounds. Suppose that in the first round "<em>Buen Kilo de Pan Flauta</em>"&nbsp;faces "<em>Melarita</em>", the former being the winner; in the second round "<em>aWArush</em>" beats "<em>Buen Kilo de Pan Flauta</em>"; and finally in the last round "<em>aWArush</em>" beats "<em>Type Mismatch</em>". Then the placement of the teams in the final scoreboard will be in the following order: 1<sup>st</sup>&nbsp;"<em>aWArush</em>", 2<sup>nd</sup>&nbsp;"<em>Type Mismatch</em>", 3<sup>rd</sup>&nbsp;"<em>Buen Kilo de Pan Flauta</em>" and 4<sup>th</sup>&nbsp;"<em>Melarita</em>".</p>
<p>To analize just how fair the new tournament format is, we will consider the teams to be numbered from <strong>1</strong>&nbsp;to <strong>N</strong>, in such a way that lower numbers represent better teams. We will assume that whenever two teams face each other in a given round, the one with the smallest number will invariably win. We would like you to help us answer the following question: What is the probability for team <strong>X</strong>&nbsp;to be placed at position <strong>Y</strong>&nbsp;in the final scoreboard?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. Each test case consists of a single line containing three integer numbers <strong>N</strong>, <strong>X</strong>&nbsp;and <strong>Y</strong>. The number <strong>N</strong>&nbsp;represents the number of teams taking part in the tournament, (<strong>2 ¡Ü&nbsp;N&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;1000</strong>), <strong>X</strong>&nbsp;represents the number of the team we are interested in, and <strong>Y</strong>&nbsp;represents its final position (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;X,Y&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing a rational number, representing the probability for team number <strong>X</strong>&nbsp;to be placed at position <strong>Y</strong>&nbsp;in the final scoreboard. Print the result with exactly <strong>4</strong>&nbsp;digits after the decimal marker, rounding if necessary.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">3 2 2
10 3 6
10 1 5
1000 1 1
1000 1000 1000</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">0.6667
0.0946
0.0000
1.0000
0.0020</span><span style="white-space: normal;">
</span></pre>