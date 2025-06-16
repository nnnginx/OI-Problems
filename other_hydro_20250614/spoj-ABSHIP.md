<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>You managed to beat your friend in Battleships and take his Internet Points! Perfectly legitimately, of course. However, for some strange reason he¡¯s upset, and now challenges you to a rematch - this time at the game of Advanced Battleships, and with even higher stakes!</p>
<p>You each have a grid consisting of $M$&nbsp;rows of $N$&nbsp;cells eacg ($1 \leq M,N \leq 500$). Each cell is either empty or contains part of a player¡¯s ship. What makes this game so ¡°advanced¡± is the fact that each ship consists of a maximal set of 1 or more adjacent, nonempty cells. Two cells are considered adjacent if they share a common side. Of course, this means that ships can have some very strange shapes. No two ships can be adjacent to one another, of course.</p>
<p>You know for a fact that you can distract your friend for a brief moment, this time by telling him that someone proved that P = NP, but this trick will again only work exactly once. While he isn¡¯t looking, you¡¯ll have time to snatch up some of his ships with one hand. Your hand can cover a square of exactly $S$x$S$&nbsp;cells ($1 \leq S \leq min\{M,N\}$), and you can gather all the ships that are at least partially within such a square at once.</p>
<p>Of course, your friend is no fool, so he¡¯s got his grid well concealed. As such, you don¡¯t know anything about it except its size, so when the time comes, you¡¯ll just choose a random square of size $S$x$S$&nbsp;that¡¯s completely within the grid.</p>
<p>As usual, these bets attract large crowds. One of the bystanders who can see your opponent¡¯s grid knows your plan, and is curious as to the expected number of ships that you will grab (in other words, the average number of ships out of all the possible snatches you could make). Nerdy though he is, he can¡¯t calculate it in his head, so he runs over to a computer and codes up a program...<strong>&nbsp;</strong></p>
<h3>Input</h3>
<p>Line $1$: 3 integers, $M$, $N$, and $S$</p>
<p>Next $M$&nbsp;lines: $N$&nbsp;characters each, representing your opponent¡¯s grid ¨C an ¡®X¡¯ represents a ship, while a ¡®.¡¯ represents an empty cell</p>
<h3>Output</h3>
<p>A single number ¨C the expected number of ships that you¡¯ll grab, rounded to 6 decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 5 2</span>
<span style="font-family: 'courier new', courier;">XXXX.</span>
<span style="font-family: 'courier new', courier;">X..X.</span>
<span style="font-family: 'courier new', courier;">X..X.</span>
<span style="font-family: 'courier new', courier;">X....</span>
<span style="font-family: 'courier new', courier;">.XX..</span></pre>
<pre><strong>Output:</strong>
</pre>
<pre><strong><span style="font-family: 'courier new', courier;">0.875000</span></strong></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>There are 16 possible areas you could pick, yielding this many ships each:</p>
<pre><span style="font-family: 'courier new', courier;">1 1 1 1</span>
<span style="font-family: 'courier new', courier;">1 0 1 1</span>
<span style="font-family: 'courier new', courier;">1 0 1 1</span>
<span style="font-family: 'courier new', courier;">2 1 1 0</span></pre>
<p>This is a total of 14 ships, for an average of 0.875 per grab.</p>