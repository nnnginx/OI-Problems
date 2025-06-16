<p>You are given an R rows x C columns grid map where each cell contains an arrow (one of the following: '^', '&gt;', '&lt;', or 'v'). If one stands on a cell, then he/she has to go to the neighbouring cell pointed by the arrow in the cell where he/she stands. Supposed you are at cell (r, c) ¨C row r and column c, then:</p>
<ul>
<li>'^' means you should go to cell (r-1, c).</li>
<li>'&gt;' means you should go to cell (r, c+1).</li>
<li>'&lt;' means you should go to cell (r, c-1).</li>
<li>'v' means you should go to cell (r+1, c).</li>
</ul>
<p>If the new cell is out of the grid map, then you fall out of the map.<br>Your task is to modify the arrows, such that if you start from any cell in the map and follow the arrows, then you will get back to the starting point. Determine the minimum number of arrows that you will have to change.</p>
<p>For example, consider the following map of 4 x 2.</p>
<p>&nbsp; &nbsp;&gt;v</p>
<p>&nbsp; &nbsp;v&lt;</p>
<p>&nbsp; &nbsp;&gt;v</p>
<p>&nbsp; &nbsp;&gt;&lt;</p>
<p>There are several ways to accomplish our goal; here are 3 solution examples:</p>
<p>&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v&lt; &nbsp; &nbsp; &gt;v</p>
<p>&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v^ &nbsp; &nbsp; ^&lt;</p>
<p>&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v^ &nbsp; &nbsp; &gt;&lt;</p>
<p>&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; &gt;^ &nbsp; &nbsp; &gt;&lt;</p>
<p>In the first solution example, we have to change 3 arrows: {(1, 2), (2, 1), (3, 2)}. In the second one, we have to change 6 arrows: {(1, 1), (1, 2), (2, 2), (3, 1), (3, 2), (4, 2)}. In the last one, we have to change 2 arrows: {(2, 1), (3, 2)}. There are many other solution examples, but among those, the minimum number of arrows you need to change is 2 (as in solution example 3).</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">If the new cell is out of the grid map, then you fall out of the map.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to modify the arrows, such that if you start from any cell in the map and follow the arrows, then you will get back to the starting point. Determine the minimum number of arrows that you will have to change.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, consider the following map of 4 x 2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;v</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;v&lt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;v</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;&lt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are several ways to accomplish our goal; here are 3 solution examples:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v&lt; &nbsp; &nbsp; &gt;v</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v^ &nbsp; &nbsp; ^&lt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; v^ &nbsp; &nbsp; &gt;&lt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp;&gt;&lt; &nbsp; &nbsp; &gt;^ &nbsp; &nbsp; &gt;&lt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first solution example, we have to change 3 arrows: {(1, 2), (2, 1), (3, 2)}. In the second one, we have to change 6 arrows: {(1, 1), (1, 2), (2, 2), (3, 1), (3, 2), (4, 2)}. In the last one, we have to change 2 arrows: {(2, 1), (3, 2)}. There are many other solution examples, but among those, the minimum number of arrows you need to change is 2 (as in solution example 3).</div>
<h3>Input</h3>
<p>The first line of input contains an integer T (T ¡Ü 100) denoting the number of cases. Each case begins with two integers R and C (1 ¡Ü R, C ¡Ü 14) denoting the number of rows and columns of the grid map. The following R lines each contains C characters (one of the following: '^', '&gt;', '&lt;', 'v') representing the arrow in each cell.</p>
<h3>Output</h3>
<p>For each case, output in a line "Case #X: Y" where X is the case number, starts from 1. and Y is the minimum number of arrows you need to change to accomplish the given goal. Output -1 for Y, if it's not possible to do so.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
4 2
&gt;v
v&lt;
&gt;v
&gt;&lt;
3 4
v&lt;&gt;v
v^^v
&gt;^^&lt;
3 4
v&lt;&lt;&lt;
v^v&lt;
&gt;&gt;&gt;^
1 2
&gt;&gt;

<strong>Output:</strong>
Case #1: 2
Case #2: 0
Case #3: 2
Case #4: 1<span style="white-space: normal;">
</span></pre>
<p><strong>Explanation:</strong></p>
<p><em>Explanation for 2<sup>nd</sup> sample case</em></p>
<p>The map already satisfies the goal; there's no need to change any arrow.</p>
<p><em>Explanation for 3<sup>rd</sup> sample case</em></p>
<p>We need to change at least 2 arrows:</p>
<p>v&lt;&gt;&lt;</p>
<p>v^v&lt;</p>
<p>&gt;^&gt;^</p>
<p><em>Explanation for 4<sup>th</sup> sample case</em></p>
<p>One arrow has to be changed:</p>
<p>&gt;&lt;</p>