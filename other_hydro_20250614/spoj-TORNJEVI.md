<p>We are being attacked on a map represented by a rectangular grid of R¡ÁS squares. The attackers are barefoot robbers, and we use small cannons on small wooden towers to defend ourselves.</p>
<p>Each tower is equipped with <strong>two cannons</strong>, placed to fire in a 90 degree angle. More precisely, cannons on one tower can be set to fire in one of the following four configurations:</p>
<ol>
<li>fire left and down;</li>
<li>fire down and right;</li>
<li>fire right and up;</li>
<li>fire up and left.</li>
</ol>
<p>A cannon ball that hits the attacker <strong>destroys him and continues to fly</strong> in the same direction. A cannon ball which hits a castle stops and does no damage to the castle (because castles are big and strong). But, when a cannon ball hits a tower, it destroys it (because towers are small and fragile).</p>
<p>We want to turn the cannons on the towers so that, when we fire exactly one shot from <strong>every cannon</strong>, <strong>we destroy all the attackers</strong>, and <strong>all our towers remain undamaged.</strong></p>
<h3>Input</h3>
<p>The first line contains two integers R and S (1 ¡Ü R, S ¡Ü 100), the dimensions of the map.</p>
<p>The next R lines contain S characters each, the map.</p>
<p>Each character on the map can be the uppercase letter '<tt>T</tt>' (tower), lowercase letter '<tt>n</tt>' (attacker), the character '<tt>#</tt>' (castle) or the character '<tt>.</tt>' (empty).</p>
<p><strong>Note:</strong> There will always be a solution, although not necessarily unique.</p>
<h3>Output</h3>
<p>Output the map in the same format as in the input, replacing '<tt>T</tt>' characters with the orientations of the cannons ¨C each tower should be replaced with one of the digits '<tt>1</tt>', '<tt>2</tt>', '<tt>3</tt>' or '<tt>4</tt>', corresponding to the four orientations as described above.</p>
<h3>Examples</h3>
<table style="width: 100%;" border="0">
<colgroup><col align="left" width="33%"> <col align="left" width="33%"> <col align="left" width="33%"> </colgroup>
<tbody>
<tr>
<td valign="top">
<pre><strong>Input:</strong>
9 13
.............
...........n.
.n.T..nnnn#..
.............
.T#n..n....T.
.............
.n.T..T....n.
.............
......n......


<strong>Output:</strong>
.............
...........n.
.n.3..nnnn#..
.............
.4#n..n....4.
.............
.n.1..2....n.
.............
......n......

</pre>
</td>
<td valign="top">
<pre><strong>Input:</strong>
5 9
.n..T..n.
.T..n....
.n..#..n.
....n..T.
.n..T..n.

<strong>Output:</strong>
.n..4..n.
.2..n....
.n..#..n.
....n..4.
.n..3..n.

</pre>
</td>
<td valign="top">
<pre><strong>Input:</strong>
9 8
n.Tnnnnn
nnnnnnTn
nTnnnnnn
nnnnTnnn
Tnnnnnnn
..#nnTnn
nnnnnnnT
nnnTn.n.
.nTnnnnn


<strong>Output:</strong>
n.3nnnnn
nnnnnn1n
n2nnnnnn
nnnn1nnn
3nnnnnnn
..#nn4nn
nnnnnnn4
nnn4n.n.
.n3nnnnn

</pre>
</td>
</tr>
</tbody>
</table>