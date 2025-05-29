<p>You are a hunter chasing a monkey in the forest, trying to shoot it down with your all-powerful automatic machine gun. The monkey is hiding somewhere behind the branches of one of the trees, out of your sight. You can aim at one of the trees and shoot; your bullets are capable of going through the branches and killing the monkey instantly if it happens to be in that tree. If it isn’t, the monkey takes advantage of the time it takes you to reload and takes a leap into a neighbouring tree without you noticing. It never stays in the same place after a shot. You would like to find out whether there is an strategy that allows you to capture the monkey for sure, irrespective of its initial location and subsequent jumps. If so, you need to determine the shortest sequence of shots guaranteeing this.</p>
<blockquote class="figure">
<div class="center">
<hr size="2">
</div>
<div class="center">
<table border="1" cellspacing="0" cellpadding="1">
<tbody>
<tr>
<td align="center"><img src="../../../content/elhipercubo:monkey1.jpg" alt="" width="300"></td>
<td align="center"><img src="../../../content/elhipercubo:monkey2.jpg" alt="" width="300"></td>
</tr>
</tbody>
</table>
</div>
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">&nbsp;</td>
</tr>
</tbody>
</table>
</div>
<a name="fig:monkey"></a>
<div class="center">
<hr size="2">
</div>
</blockquote>
<p>As an example, consider the situation in which there are only two neighboring trees in the forest (left hand side of the figure). It is then possible to make sure you capture the monkey by shooting twice at the same tree. Your first shot succeeds if the monkey happened to be there in the first place. Otherwise, the monkey was behind the other tree and it will necessarily have moved when you shoot for the second time.</p>
<p>However, depending on the shape of the forest it may not be possible for you to ensure victory. One example of this is if there are three trees, all connected to one another (right hand side of the figure). No matter where you aim at, there are always two possible locations for the monkey at any given moment. (Note that here we are concerned with the worst-case scenario where the monkey may consistently guess your next target tree).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of several test cases, separated by single blank lines. Each test case begins with a line containing two integers <em>n</em> and <em>m</em> (1 ≤ <em>n</em> ≤ 21); <em>n</em> is the number of trees in the forest, and <em>m</em> is the number of adjacency relations between trees.  Each of the following <em>m</em> lines contains two distinct integers between 0 and <em>n</em>−1 (inclusive), the identifiers of the trees in an adjacent pair. The order of both trees within a pair carries no meaning, and no pair appears more than once. You may further assume that no tree is adjacent to itself, and there is always a path between any two trees in the forest.</p>
<p>The test cases will finish with a line containing only two zeros (also preceded with a blank line).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>Print a line for each test case. The line should contain the single word <tt>Impossible</tt> if the task is impossible. Otherwise, it must contain the shortest sequence of shots with the required property, in the format <em>L</em>: <em>V</em><sub>1</sub> <em>V</em><sub>2</sub> … <em>V</em><sub><em>L</em></sub>, where <em>L</em> is the length of the sequence, and <em>V</em><sub>1</sub>, <em>V</em><sub>2</sub>, …, <em>V</em><sub><em>L</em></sub> are space-separated integers containing the identifiers of the trees to shoot at in the right order. If several shortest sequences exist, print the lexicographically smallest one. (A sequence is smaller than another in lexicographic order if the first element on which they differ is smaller in the first one).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2 1
0 1

3 3
0 1
1 2
2 0

4 3
0 1
2 3
1 3

0 0
</pre>
</div>
<p><br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2: 0 0
Impossible
4: 1 3 3 1
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Marçal Garolera Huguet</em></blockquote>