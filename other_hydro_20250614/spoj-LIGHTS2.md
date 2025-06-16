<p>John has <em>n</em> light bulbs and a switchboard with <em>n</em> switches; each bulb can be either on or off, and pressing the <em>i</em>−th switch changes the state of bulb <em>i</em> from on to off, and viceversa. He is using them to play a game he has made up. In each move, John selects a (possibly empty) set of switches and presses them, thus inverting the states of the corresponding bulbs. Initially all lights are off, and after exactly <em>m</em> moves John would like to have the first <em>v</em> bulbs on and the rest off; otherwise he loses the game. There is only one restriction: he is not allowed to press the same <em>set</em> of switches in two different moves.</p>
<p>This is quite an easy game, as there are lots of ways of winning. This has encouraged him to keep playing different winning games, and now he is intent on trying them all. Help him count how many ways of winning there are. Two games are considered the same if, after a reordering of the moves in one of them, at every step the same set of switches is pressed in both of them.</p>
<p>For example, if <em>n</em> = 4, <em>m</em> = 3, and <em>v</em> = 2, one possible winning game is obtained by pressing switches 1, 2 and 4 in the first move, 1 and 3 in the second one, and 1, 3 and 4 in the last one. This is considered equivalent to, say, first pressing 1 and 3; then 1, 2, 4; and then 1, 3, 4.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input has at most 500 lines, one for each test case. Each line contains three integers <em>n</em> (1 ≤ <em>n</em> ≤ 1&nbsp;000), <em>m</em> (1 ≤ <em>m</em> ≤ 1&nbsp;000), and <em>v</em> (0 ≤ <em>v</em> ≤ <em>n</em>). The last line of input will hold the values <tt>0 0 0</tt> and must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>Print one line for each test case containing the number of ways John can play the game, modulo the prime 10&nbsp;567&nbsp;201.</p>
<p><br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3 3 1
6 4 0
6 4 3
0 0 0
</pre>
</div>
<p><br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">7
10416
9920
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David García Soriano</em><em></em></blockquote>