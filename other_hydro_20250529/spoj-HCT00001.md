<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Rij¨¦l is a very wise teacher. He loves mathematics, especially games and geometry problems. Recently one of his students challenged him to the following game:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Initially, there is a polygon with N vertices drawn in the plane. The polygon is strictly convex, i.e., each internal angle is strictly smaller than 180 degrees. The vertices of the polygon are numbered 1 through N, in clockwise order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Two players play the game on this polygon. The players take alternating turns. In each turn, the current player chooses a diagonal or a side of the polygon and draws it as a straight line segment. (A diagonal of the polygon is a line segment that connects any two non-adjacent vertices of the polygon.) The player is only allowed to choose a diagonal or a side that does not intersect any of the previously drawn segments (it must not share endpoints with any of them either). The player who cannot draw a diagonal or a side according to the above rules loses the game.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given the int N.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We assume that both players play the game optimally. Return 1 if the first player wins and 2 otherwise.</div>
<p>Rij¨¦l is a very wise teacher. He loves mathematics, especially games and geometry problems. Recently one of his students challenged him to the following game:</p>
<p>Initially, there is a polygon with N vertices drawn in the plane. The polygon is strictly convex, i.e., each internal angle is strictly smaller than 180 degrees. The vertices of the polygon are numbered 1 through N, in clockwise order.</p>
<p>Two players play the game on this polygon. The players take alternating turns. In each turn, the current player chooses a diagonal or a side of the polygon and draws it as a straight line segment. (A diagonal of the polygon is a line segment that connects any two non-adjacent vertices of the polygon.) The player is only allowed to choose a diagonal or a side that does not intersect any of the previously drawn segments (it must not share endpoints with any of them either). The player who cannot draw a diagonal or a side according to the above rules loses the game.</p>
<p>&nbsp;</p>
<p>You are given the int N.</p>
<p>We assume that both players play the game optimally. Return 1 if the first player wins and 2 otherwise.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The only line of input contains N (1&nbsp;&nbsp;¡Ü N&nbsp;&nbsp;¡Ü 1000), the number of vertices of the polygon.</p>
<h3>Output</h3>
<p>Print 1 if the first player wins, or 2 otherwise.</p>
<h3>Example</h3>
<pre><strong><table border="0"><tbody><tr><td>Input</td><td>Output</td></tr><tr><td>3</td><td>1</td></tr><tr><td>4</td><td>1</td></tr><tr><td>15</td><td>2</td></tr></tbody></table><br></strong></pre>