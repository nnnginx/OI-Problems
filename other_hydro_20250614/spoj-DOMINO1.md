<p>You are given N domino tiles. Each tile is made of some number of squares (not necessarily two), and each square is coloured either white or black (we use the Croatian letters: B for white and C for black).</p>
<p>Find the longest chain that can be made of these tiles. Each tile can be used at most once and cannot be rotated (for example, BC cannot become CB). The chain is made by a common rule: in adjacent tiles, touching squares must be of the same colour.</p>
<h3>Input</h3>
<p>[N ��&nbsp;100, the number of dominoes]</p>
<p>in the next N lines:</p>
<p>[a string of size between 1 and 100, representing the domino]</p>
<h3>Output</h3>
<p>The length of the longest chain.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">4
CB
BCC
BBCC
BCBBC</pre>
<strong>Output:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">11</pre>
</pre>