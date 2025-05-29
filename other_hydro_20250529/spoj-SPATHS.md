<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Nikola lives in Bittown and he is in love with his girlfriend Anita from a town called Hextown. Nikola</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">knows the country map very well, and he found the shortest path between these two towns. He calls</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">this path lucky path. The map of the country can be described as a collection of towns connected</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">with bidirectional roads.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">One day the president of this country decided that there are going to be some works on the roads. In</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">order to uphold the traffic in the country, only one road is going to be closed per day.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each road on the lucky path, Nikola wants to know the length of the shortest path between Anita</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and him if that road is closed.</div>
<p>Nikola lives in Bittown and he is in love with his girlfriend Anita from a town called Hextown. Nikola</p>
<p>knows the country map very well, and he found the shortest path between these two towns. He calls</p>
<p>this path lucky path. The map of the country can be described as a collection of towns connected</p>
<p>with bidirectional roads.</p>
<p>One day the president of this country decided that there are going to be some works on the roads. In</p>
<p>order to uphold the traffic in the country, only one road is going to be closed per day.</p>
<p>For each road on the lucky path, Nikola wants to know the length of the shortest path between Anita</p>
<p>and him if that road is closed.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of input contains four integers : n - the number of cities, m - the number of roads</p>
<p>between these towns, a - index of town Bittown where Nikola lives, b - the index of town</p>
<p>Hextown where Anita lives. Towns are indexed with numbers 1, 2,¡­, n. Next m lines specify roads :</p>
<p>each line contains three integers : u, v and w - there exist road between towns u and v with length w.</p>
<p>Last line of the input contains number k followed by k numbers a = v<sub>1</sub>, v<sub>2</sub>, ¡­, v<sub>k</sub> = b - the lucky path</p>
<p>that Nikola uses.&nbsp;</p>
<h3>Output</h3>
<p>For every integer t = 1 ¡­ k - 1, in separate line, print the length of the shortest path between cities a</p>
<p>and b, if the road (v<sub>t</sub>, v<sub>t + 1</sub>) is closed. If there is no such path, output ¡°-1¡± without quotes.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 6 1 5
1 2 1
2 3 3
2 5 100
3 4 3
3 5 5
4 5 3
4 1 2 3 5

<strong>Output:</strong>
-1
101
10
</pre>
<pre><h3>Constraints</h3><em>-<span style="white-space: pre;">	</span>1 ¡Ü n ¡Ü 2000, 1 ¡Ü m ¡Ü 100.000
-<span style="white-space: pre;">	</span>1 ¡Ü a, b ¡Ü n
-<span style="white-space: pre;">	</span>1 ¡Ü w ¡Ü 100.000
-<span style="white-space: pre;">	</span>There is at most one road between each pair of cities.
-<span style="white-space: pre;">	</span>You may assume that the given path is one of the shortest paths that connects given two
cities a and b.</em></pre>