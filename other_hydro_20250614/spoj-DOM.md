<p><em>Original problem statement (in Polish) can be found <a href="https://pizza.natodia.net/static/tasks/2016/eliminations/efekt.pdf">here</a>.</em></p>
<p>Dominik "Domino" Doma¨½ski is a scientist. He's conducting research on quantum physics. Lately, he started taking a closer look at certain very interesting effect, which can be observed when some quantum objects interact.</p>
<p>In his next experiment, he placed <strong>n</strong> infinitely thin lines on the table, perpendicularly to the surface, in a row. Lines have different heights, distances between the lines can also differ. (Dominik calls these lines "domino tiles"). Looking from the front, they look like <strong>n</strong> segments, standing vertically on the X axis of the Cartesian coordinate system.</p>
<p>Domino tiles can be toppled. If a tile has a height of <strong>h</strong>, it will topple other tiles at most <strong>h</strong> units away. More precisely, if tile is placed at the position <strong>x</strong>, and is knocked over to the right, it will topple the tiles placed at positions <strong>x</strong>+1, <strong>x</strong>+2, ..., <strong>x</strong>+<strong>h</strong>. If this tile is knocked over to the left, it will topple the tiles at positions <strong>x</strong>-1, <strong>x</strong>-2, ..., <strong>x</strong>-<strong>h</strong>.</p>
<p>Dominik observed a very interesting phenomenon, which he called "Domino's effect" - toppling one domino tile can cause other tiles to topple, which can in turn topple other tiles. He started to wonder how to take advantage of this effect in a best possible way. What is the minimum number of tiles that need to be toppled, in order for all the dominoes to fall?</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, testcases follow.</p>
<p>The description of a single testcase begins with a single integer <strong>n</strong> (1 &lt;= <strong>n</strong> &lt;= 1000) - the number of domino tiles in an arrangement.</p>
<p>It is followed by <strong>n</strong> integers <strong>h<sub>i</sub></strong> - heights of subsequent tiles.</p>
<p>It ends with <strong>n</strong>-1 integers <strong>d<sub>i</sub></strong> - distances between neighboring tiles.</p>
<p>(1 &lt;= <strong>h<sub>i</sub></strong>, <strong>d<sub>i</sub></strong> &lt;= 10<sup>6</sup>).</p>
<h3>Output</h3>
<p>For every testcase you should find a sequence of domino tiles, that will knock down the whole arrangement. It should begin with an integer <strong>k</strong> (1 &lt;= <strong>k</strong> &lt;= <strong>n</strong>), denoting the number of tiles to be pushed. Then, descriptions of moves should follow. One move is described by one integer <strong>x<sub>i</sub></strong> (1 &lt;= <strong>x<sub>i</sub></strong> &lt;= <strong>n</strong>) and one letter (either L or P). It means that during the <strong>i</strong>-th move, we topple a tile number <strong>x<sub>i</sub></strong> (counting from 1, according to original arrangement). L means that we knock it over to the left, P means knocking over to the right.</p>
<p>The sequence should knock over all the tiles, while using as few moves as possible.</p>
<h3>Example</h3>
<p>Input:</p>
<pre>1
6
1 5 1 1 1 1
2 1 2 1 1</pre>
<p>Output:</p>
<pre>2
2 P
1 L</pre>
<h3>Explanation</h3>
<p>First we topple the domino tile number 2 (of length 5) to the right, which knocks over everything to the right of that tile. Then, we topple tile number 1 - the only one that remains.</p>