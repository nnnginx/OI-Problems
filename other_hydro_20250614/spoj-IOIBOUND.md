<p>Farmer Don watches the fence that surrounds his N meter by N meter square, flat field (2&lt;=N&lt;=500,000). One fence corner is at the origin (0, 0) and the opposite corner is at (N,N); the sides of Farmer Don's fence are parallel to the X and Y axes.Fence posts appear at all four corners and also at every meter along each side of the&nbsp;fence, for a total of 4×N fence posts. The fence posts are vertical and are considered to&nbsp;have no radius. Farmer Don wants to determine how many of his fence posts he can&nbsp;watch when he stands at a given location within his fence.&nbsp;Farmer Don’s field contains R (1&lt;=R&lt;=30,000) huge rocks that obscure his view of some&nbsp;fence posts, as he is not tall enough to look over any of these rocks. The base of each&nbsp;rock is a convex polygon with nonzero area whose vertices are at integer coordinates.&nbsp;The rocks stand completely vertical. Rocks do not overlap, do not touch other rocks, and&nbsp;do not touch Farmer Don or the fence. Farmer Don does not touch the fence, does not&nbsp;stand within a rock, and does not stand on a rock.&nbsp;Given the size of Farmer Don's fence, the locations and shapes of the rocks within it, and&nbsp;the location where Farmer Don stands, compute the number of fence posts that Farmer&nbsp;Don can see. If a vertex of a rock lines up perfectly with a fence post from Farmer Don's&nbsp;location, he is not able to see that fence post.</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line of input contains two space-separated integers: N and R.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">· The next line of input contains two space-separated integers that specify the X</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and Y coordinates of Farmer Don's location inside the fence.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">· The rest of the input file describes the R rocks:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">o Rock i’s description starts with a line containing a single integer pi (3 £ pi</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">£ 20), the number of vertices in the rock's base.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">o Each of the next pi lines contains a space-separated pair of integers that are</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the X and Y coordinates of a vertex. The vertices of a rock’s base are</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">distinct and given in counterclockwise order.</div>
<p>The first line of input contains two space-separated integers: N and R.&nbsp;The next line of input contains two space-separated integers that specify the X&nbsp;and Y coordinates of Farmer Don's location inside the fence.&nbsp;The rest of the input file describes the R rocks:&nbsp;Rock i’s description starts with a line containing a single integer pi (3&lt;=pi&lt;=20), the number of vertices in the rock's base.&nbsp;Each of the next pi lines contains a space-separated pair of integers that are&nbsp;the X and Y coordinates of a vertex. The vertices of a rock’s base are&nbsp;distinct and given in counterclockwise order.</p>
<h3>Output</h3>
<p>The output file should contain a single line with a single integer, the number of fence&nbsp;posts visible to Farmer Don.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
100 1
60 50
5
70 40
75 40
80 40
80 50
70 60

<strong>Output:</strong>
319</pre>