<p>Bored to death working at the Byteland Office...your colleagues have resorted to game of crosses Xs and naughtd Os or Tic-tac-toe. One of them keeps on losing and is tired of the jokes. He plans to have an Android app in his phone to help him out. He is your good friend and seeks your assistance. "Treat at ANC is guaranteed", he says.</p>
<p>He also is very frugal when it comes to memory usage. So please don't write a long if else chain...cause you have to do the task within 999 bytes</p>
<h3>Input</h3>
<p>An integer T - the number of test cases. (T&lt;1000). T test cases follow.</p>
<p>Each test case comprises 3 strings each separated by newline and containing exactly 3 characters(either 'X','O' or '_') per line. An empty line follows each test case. Each input position is guaranteed to be a valid tic tac toe position such that the game is still not over.</p>
<h3>Output</h3>
<p>For each test case print "WON"&nbsp;if it is a sure shot winning position. Else print "CONTINUE". Then output the game after having made your move. If more than one move are equally good try playing the move on the first empty spot.</p>
<h3>Example</h3>
<h3><strong>Input:</strong></h3>
<pre>2
OOX
OX_
__X

XX_
XOO
_O_

</pre>
<h3><strong>Output:</strong></h3>
<pre>WON
OOX
OXX
__X
WON
XXX
XOO
_O_
</pre>
<pre><span style="white-space: normal;"><h3>Info</h3></span><span style="color: #000020; white-space: normal; background-color: #e8edd0;">1) i</span><span style="color: #000020; white-space: normal; background-color: #e8edd0;">guaranteed always to be X's move (i</span><span style="color: #000020; white-space: normal; background-color: #e8edd0;">t is the standard) and whose move it currently is can be computed...&nbsp;</span></pre>
<pre><span style="color: #000020; white-space: normal; background-color: #e8edd0;">2) winning position is meant for the current player&nbsp;<br></span><span style="color: #000020; white-space: normal; background-color: #e8edd0;">3) winning in lesser number of moves is better and drawing is better than losing as in general AI&nbsp;<br></span><span style="color: #000020; white-space: normal; background-color: #e8edd0;">4) you need to print the board as it looks after making the best move&nbsp;</span></pre>
<pre><span style="color: #000020; white-space: normal; background-color: #e8edd0;">5) print WIN if the current player can win in the case when both players play optimally from here on...&nbsp;</span></pre>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 312px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">__X</div></pre>