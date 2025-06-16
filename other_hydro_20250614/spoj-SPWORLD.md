<p align="center"><strong><br></strong></p>
<p>Avatar Korra is trapped in the spirit world and she summons Avatar Aang for help. Avatar Aang who wants to help Avatar Korra first wants to know whether she is intelligent enough to win the ancient game of co-prime Polygons. Two polygons are said to be co-prime if the number of their sides is co-prime. Examples - A 3-sided polygon and a 4-sided polygon are co-prime whereas a 4 sided polygon and a 6 sided polygon are not. The game begins with N polygons. The game has the following rules-</p>
<ol>
<li>A player takes any one polygon cuts them into two co-prime polygons. Cutting is done along a line joining 2 vertices of a polygon (points cannot be adjacent). These 2 new co-prime polygons now become a part of the game. If he/she is not able to perform such a cut on any of polygons he/she loses.</li>
<li>Avatar Aang takes the first turn. After each cut it is the turn of the other person. In a turn a person can make only one cut.</li>
<li>Though Aang thinks Korra is not intelligent he is forgetting that she has the wisdom of all the Avatars, even him. So she knows the game. Hence both of them play optimally.</li>
</ol>
<p><strong>Input</strong></p>
<p>The first line contains the number of test cases (T) followed by T lines each containing a test case. A test case begins with the number N. N integers follow denoting the number of sides in the N polygons. Every polygon will has at least 3 sides.</p>
<p><strong>Output</strong></p>
<p>For each test case output the winner of the game.</p>
<p><strong>Constraints </strong>T&lt;=15, N&lt;=7, 3&lt;=sides of polygon&lt;=1000</p>
<p><strong>Sample Input</strong></p>
<p>2</p>
<p>3 5 6 7</p>
<p>2 6 7</p>
<p><strong>Sample Output</strong></p>
<p>Aang</p>
<p>Korra</p>