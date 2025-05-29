<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Don Cherry has been hired to run 24-hour coverage of a series of single-elimination, bracket-style, furniture disassembly tourneys (tournaments). Each competitor has a furniture disassembly skill level, an integer between $1$ and $10^9$. In every head-to-head match, the competitor with the larger skill level wins and moves on, while the other is eliminated from the tourney. It is guaranteed that, at any time, the skill levels of all competitors are distinct, so there are no ties.</p>
<p>There are $2^N$ ($1 \leq N \leq 20$) competitor positions in the tourney tree, numbered $1, 2, \ldots, 2^N$ from left to right. In the first round, competitors 1 and 2 face off in a furniture disassembly race, as do competitors 3 and 4, etc. In each subsequent round, the winners of the first two matches from the previous round compete, as do the winners of the following two, etc. After $N$ rounds, a single winner remains. For example, when $N=2$, the tourney tree looks like this:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:tourney1.bmp" alt=""></p>
<p>where A represents the winner of the match between competitors 1 and 2, B represents the winner of the match between competitors 3 and 4, and C represents the winner of the match between A and B. The winner of this tourney is C.</p>
<p>Because of sponsorship contracts, some competitors will be replaced over time. After any new person comes in, a new tourney is held.</p>
<p>In order to help Don Cherry, you must write a program to compute certain tourney statistics at various points in time, given a sequence of $M$ ($1 \leq M \leq 10^6$) commands - see the input format below.</p>
<h3>Input</h3>
<p>The first line of input contains two integers, $N$ and $M$.</p>
<p>The next $2^N$ lines, for $i$ from $1$ to $2^N$, each contain one integer $S_i$, indicating the skill level of the initial competitor at position $i$ in the tourney tree.</p>
<p>Each of the following $M$ lines will be a command in one of three formats:</p>
<ul>
<li>"<strong>R</strong> $i$ $s$" means that the competitor at position $i$ is removed, and replaced with a new one with skill level $s$. A new tourney should then be held.</li>
<li>"<strong>W</strong>" means that your program should determine who won the current tourney. Print out the position $i$ (between $1$ and $2^N$) of this competitor.</li>
<li>"<strong>S</strong>&nbsp;$i$" means that your program should print out the number of rounds that the competitor at position $i$ won in the current tourney.</li>
</ul>
<h3>Output</h3>
<p>For each "<strong>W</strong>" or "<strong>S</strong>&nbsp;$i$" command in the input, print out the corresponding integer on a line by itself.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2 8<br>30<br>20<br>10<br>40<br>S 1<br>W<br>R 4 9<br>S 4<br>W<br>R 2 35<br>S 2<br>W</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>4<br>0<br>1<br>2<br>2</span></pre>
<pre><span style="font-weight: bold;">Explanation of Sample:</span></pre>
<p>The results of the initial tourney are as follows:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:tourney2.bmp" alt=""></p>
<p>As can be seen, competitor 1 wins 1 match, and competitor 4 wins the entire tourney. After this, competitor 4 is replaced by a new competitor with skill level 9. As can be seen below, this causes a different outcome for the tourney held after the third command:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:tourney3.bmp" alt=""></p>
<p>Finally, the state of the tourney tree after the next competitor replacement (caused by the sixth command) is:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:tourney4.bmp" alt=""></p>