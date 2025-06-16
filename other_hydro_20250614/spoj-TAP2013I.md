<p><strong><em>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</em></strong></p>
<p>Finding the treasures hidden centuries ago by the pirates of the Caribbean islands is no easy task, but even more difficult is living to tell the story. This is because, as everybody knows, pirates had supernatural powers which they used to curse the person who took their treasure unauthorized.</p>
<p>A very common curse among the most powerful of pirates, and for which it is always a good idea to be prepared, is known today as the <em>deadly mist</em>. Whenever a pirate's treasure is found, this curse will make a poisonous mist lift from the ground until the whole island gets covered by it. Any living creature that is touched by the mist will die instantly, something especially undesirable for those who have just found a treasure. The only way to save yourself is then to return to your boat, always going through areas that have not yet been covered by the mist, and thus flee with that part of the treasure that may have been rescued. In this problem we are interested in knowing what's the maximum amount of time that one can take to collect the treasure in such a way so as to be able to return to the boat alive.</p>
<p>To simplify the problem, we will consider that an island can be represented by a grid with <strong>R</strong> rows and <strong>C</strong> columns, in which the cell in the <strong>i</strong>-th row and the <strong>j</strong>-th column has height <strong>H<sub>ij</sub></strong>&nbsp;above sea level. Furthermore, we will assume that the treasure is always hidden in the cell in row <strong>1</strong> and column <strong>1</strong>, because this is the one furthest away from the only place where the boat can set anchor, which is the cell in row <strong>R</strong> and column <strong>C</strong>. The deadly mist appears at sea level at the very same instant that the treasure is found, and then rises on all the island at a rate of one unit of height per second, so that after <strong>t</strong> seconds one cannot be in any cell of height less or equal to <strong>t</strong>. In order to return to the boat, you may go from one cell to another only if they share a side, so that if you are on a given cell you can only move horizontally to the cell before or after it in the same row, or vertically to the cell before or after it in the same column, but you cannot move diagonally or cross the boundaries of the island. Each such movement from one cell to another takes exactly one second.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integer numbers <strong>R</strong> and <strong>C</strong>, respectively the number of rows and columns of the grid that represents the island, which consists of at least two cells (<strong>1 ¡Ü&nbsp;R, C <strong>¡Ü</strong>&nbsp;500</strong> and <strong>R¡ÁC ¡Ý&nbsp;2</strong>). Each of the following <strong>R</strong> lines contains <strong>C</strong> values. In the <strong>i</strong>-th of these <strong>R</strong> lines, the <strong>j</strong>-th value is an integer <strong>H<sub>ij</sub></strong>&nbsp;representing the height of the cell at row <strong>i</strong> and column <strong>j</strong> (<strong>1 <strong><strong>¡Ü</strong></strong>&nbsp;H<sub>ij</sub>&nbsp;<strong><strong>¡Ü</strong></strong>&nbsp;10<sup>6</sup></strong> for <strong>i = 1, ..., R</strong> and <strong>j = 1, ..., C</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a single line containing an integer number representing the maximum amount of time in seconds that one can take to collect the treasure, so as to be able to return to the boat without being reached by the deadly mist. Print the number <strong>-1</strong> if it is impossible to return to the boat even if one starts the way back as soon as the treasure is discovered.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 273px; width: 1px; height: 1px; overflow: hidden;">3 3</div><span style="font-family: 'courier new', courier;">3 3
2 3 4
3 4 5
4 5 6</span></pre>
<pre><strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3 3
1 2 3
2 2 3
2 4 5</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">-1</span></pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3 2
1000000 1000000
1000000 1000000
1000000 314</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">310</span><span style="white-space: normal;">&nbsp;</span></pre>