<p>One day Rashad and Mahmud were talking about Nim and other mathematical games while teaching game theory to their students. Ibrahim, as usual, solved all problems after the lecture, so teachers decided to give a hard task to him:</p>
<p>Ziya the ProGamer (yes, you know him from my <a href="http://www.spoj.com/problems/HUSGAME/">this problem</a>) and Rafael a.k.a. Farael are playing a game with two piles that have <strong><em>A</em></strong> coins in first one, and <strong><em>B</em></strong> coins in the latter. Of course, Ziya starts first and they take alternating turns making the following moves: The player whose turn is; picks one pile with <strong>at least two</strong> coins, removes from that pile <strong><em>x</em></strong> coins for some <strong><em>2 ¡Ü x ¡Ü 4</em></strong>, and adds one coin to another pile. Players can choose different <strong><em>x</em></strong> in each move, and who cannot make move loses. As you know, Ziya is ProGamer (don't confuse with Programmer!!), and Rafael is Farael (that special name helps him to make the best move possible!!)<strong> </strong>they both play perfectly.</p>
<p>Ibrahim thought about a dynamic programming solution for this task but the constraints for the task baffled him. The only idea in his mind is observing the answer, however, he thinks that his solution is not enough for this task, so your help is needed here. Please, answer some queries that Ibrahim wants to know.</p>
<p><strong>Input</strong></p>
<p>The first line of the input consisting of the number of the queries Ibrahim will ask - <strong>T (1 ¡Ü T ¡Ü 5000).</strong> For each query, there are given two numbers, <strong><em>A</em></strong> and <strong><em>B</em></strong> <strong>(1 ¡Ü A, B ¡Ü 10<sup>18</sup>; a little long game, huh?)</strong> in a separate line.</p>
<p><strong>Output</strong></p>
<p>For each query of Ibrahim, print "Ziya" if Ziya will win the game, "Farael" otherwise, in separate line.</p>
<p><span style="font-size: medium;"><strong>Example</strong></span></p>
<p><span style="font-size: small;"><strong>Input:</strong></span></p>
<pre>3
1 5
2 3
4 12</pre>
<p><span style="font-size: small;"><strong>Output:</strong></span></p>
<pre>Ziya
Farael
Farael</pre>

Note: Please, read the statement again (23.06.2018).