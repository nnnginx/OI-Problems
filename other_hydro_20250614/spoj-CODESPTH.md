<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Consider a regular polygon with N vertices labelled 1..N. In how many ways can you draw K diagonals such that no two diagonals intersect at a point strictly inside the polygon? A diagonal is a line segment joining two non adjacent vertices of the polygon.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. Each of the next T lines contain two integers N and K.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one corresponding to each test case. Since the answer can be really huge, output it modulo 1000003.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 10000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 &lt;= N &lt;= 10^9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= K &lt;= N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Explanation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the first case, there are clearly 2 ways to draw 1 diagonal - 1 to 3, or 2 to 4. (Assuming the vertices are labelled 1..N in cyclic order).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the third case, at most 2 non-intersecting diagonals can be drawn in a 5-gon, and so the answer is 0.</div>
<p>&nbsp;</p>
<p>Consider a regular polygon with N vertices labelled 1..N. In how many ways can you draw K diagonals such that no two diagonals intersect at a point strictly inside the polygon? A diagonal is a line segment joining two non adjacent vertices of the polygon.</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. Each of the next T lines contain two integers N and K.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines, one corresponding to each test case. Since the answer can be really huge, output it modulo 1000003.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 10000</p>
<p>4 &lt;= N &lt;= 10^9</p>
<p>1 &lt;= K &lt;= N</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3</p>
<p>4 1</p>
<p>5 2</p>
<p>5 3</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2</p>
<p>5</p>
<p>0</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p>For the first case, there are clearly 2 ways to draw 1 diagonal - 1 to 3, or 2 to 4. (Assuming the vertices are labelled 1..N in cyclic order).</p>
<p>For the third case, at most 2 non-intersecting diagonals can be drawn in a 5-gon, and so the answer is 0.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>