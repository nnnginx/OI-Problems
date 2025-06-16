<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>You and a friend are playing the classic game of Battleships. You each have a grid consisting of $M$ rows of $N$ cells each ($1 \leq M,N \leq 2000$). Each cell is either empty or contains a player¡¯s ship (in this version of the game, all ships are the size of one cell). The goal of the game is to destroy all of the opponent¡¯s ships by hitting individual cells.</p>
<p>You and your friend have bet tons of Internet Points on this game. Unfortunately, your friend is completely owning you. So desperate times call for desperate measures.</p>
<p>You know for a fact that you can distract your friend for a brief moment by telling him that a famous programmer is behind him, but this trick will only work exactly once (programmers are so predictable). While he isn¡¯t looking, you¡¯ll have time to snatch up some of his ships with one hand. Your hand can cover a square of exactly $S$x$S$ cells ($1 \leq S \leq min\{M,N\}$), and you can gather all the ships within such a square at once.</p>
<p>Of course, your friend is no fool, so he¡¯s got his grid well concealed. As such, you don¡¯t know anything about it except its size, so when the time comes, you¡¯ll just choose a random square of size $S$x$S$ that¡¯s completely within the grid.</p>
<p>As usual, these bets attract large crowds. One of the bystanders who can see your opponent¡¯s grid knows your plan, and is curious as to the expected number of ships that you will grab (in other words, the average number of ships out of all the possible snatches you could make). Nerdy though he is, he can¡¯t calculate it in his head, so he runs over to a computer and codes up a program...</p>
<p><strong>&nbsp;</strong></p>
<h3>Input</h3>
<p>Line $1$: 3 integers, $M$, $N$, and $S$</p>
<p>Next $M$ lines: $N$ characters each, representing your opponent¡¯s grid ¨C an ¡®X¡¯ represents a ship, while a ¡®.¡¯ represents an empty cell</p>
<h3>Output</h3>
<p>A single number ¨C the expected number of ships that you¡¯ll grab, rounded to 6 decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3 4 2</span>
<span style="font-family: 'courier new', courier;">XX.X</span>
<span style="font-family: 'courier new', courier;">XX..</span>
<span style="font-family: 'courier new', courier;">.X..</span></pre>
<pre><strong>Output:</strong>
</pre>
<pre><strong><span style="font-family: 'courier new', courier;">2.000000</span></strong></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>There are 6 possible areas you could pick, yielding this many ships each:</p>
<pre><span style="font-family: 'courier new', courier;">4 2 1</span>
<span style="font-family: 'courier new', courier;">3 2 0</span></pre>
<p>This is a total of 12 ships, for an average of exactly 2 per grab.</p>