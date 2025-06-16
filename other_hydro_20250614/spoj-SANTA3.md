<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Santa's favourite part of Christmas is, of course, entering people's houses through their fireplaces at night and leaving them presents. On this occasion, he's visiting a house which can be modeled as a rectangular grid of cells, with $R$ ($1 \leq R \leq 100$) rows and $C$ ($1 \leq C \leq 100$) columns. Each cell is either empty (represented by a '.'), contains a wall ('#'), contains a fireplace ('F'), contains a stocking of a certain size ('1'..'9'), or is empty but initially contains a dog facing in a certain direction (with up represented by '^', right by '&gt;', down by 'v', and left by '&lt;'). Exactly one cell contains a fireplace, and this is where Santa begins his business.</p>
<p>Based on the layout of the house, Santa has devised a plan of action in advance. He will enter carrying $P$ ($1 \leq P \leq 10^9$) presents, and will proceed to execute $M$ ($1 \leq M \leq 1000$) moves in order, one each second. Each move consists of moving one cell up (represented by a 'U'), right ('R'), down ('D'), or left ('L'). However, Santa cannot walk through walls, so if he would move outside the grid, or if the cell that he would move into contains a wall, he stays put for the second.</p>
<p>Each second, just as Santa is making his move, all of the dogs in the house also move simultaneously. Each dog moves forward one cell in the direction that it's facing, if that cell is within the grid and is empty (ignoring other dogs or Santa). Otherwise, it rotates clockwise by 90 degrees. Note that dogs don't interfere with one another in any way, and at various points in time there may be multiple dogs in a single cell.</p>
<p>Now, at the end of the second, if Santa finds himself in a cell with a stocking, he deposits a single present in it, if possible. In particular, he must be carrying at least one present, and the stocking must not have already been stuffed with a number of gifts equal to its capacity. Otherwise, if Santa is in the cell containing the fireplace, he immediately exits the house <em>if</em> he has no presents left, and/or he has already placed at least one present into every stocking in the house. Finally, if Santa finds himself in the same cell as one or more dogs, each such dog in turn steals half of his remaining presents, rounded up.</p>
<p>Before executing his brilliant plan, Santa would like to know how well his excursion will actually go. He'd like you to make a copy of the grid representing the house, but with every cell containing a stocking labelled with a digit ('0'..'9') representing how many presents that stocking will contain in the end, and with every other cell represented by just a '.'. He'd also like to know where in the house he'll end up.</p>
<h3>Input</h3>
<p>First line: $R$ and $C$</p>
<p>Next $R$ lines: $C$ characters, representing the $i$th row of the grid as described above, for $i=1..R$</p>
<p>Next line: $M$ and $P$</p>
<p>Next line: $M$ characters, representing Santa's moves</p>
<h3>Output</h3>
<p>$R$ lines: $C$ characters, representing the distribution of presents in the $i$th row of the grid as described above, for $i=1..R$</p>
<p>Next line: The row and column of the last cell which Santa will visit</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 3<br>.1.<br>#F3<br>#9.<br>..1<br>..&lt;<br>10 4<br>RRDDDULUUU</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">.0.<br>..2<br>.0.<br>..1<br>...<br>2 2</span>&nbsp;</pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>After his first move, Santa ends up at coordinates (2,3) (the 3rd cell in the 2nd row), and deposits one present there. During his second move, he stays in that cell due to hitting the right wall of the house, and so he deposits another gift in the stocking.</p>
<p>After 2 more seconds, he reaches the stocking at coordinates (4,3), and fills it up with a present. He returns to this cell 2 seconds later, but cannot put his last gift in the stocking because it's full.</p>
<p>On his next move, Santa encounters a dog at coordinates (4,2). Before this, the dog had moved left to (5,1), rotated, moved up to (4,1), rotated, and moved to (4,2) after 6 seconds - when Santa arrives after 7 seconds, the dog is still in this cell, rotating to face downwards. As such, Santa loses his only remaining present to it.</p>
<p>He next moves up to coordinates (3,2), but cannot deposit any presents in the stocking there because he has none. Finally, he moves up to the fireplace at coordinates (2,2), at which point he exits the house without ever making the final move up to (1,2).</p>