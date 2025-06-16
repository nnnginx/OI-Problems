<p>Recently Zippy received a puzzle. It is an n*m matrix. In each cell of the matrix, there is a switch and a light. Once he flips the switch in a cell, lights in the same column or the same row as the cell (including itself) change to its opposite state (which means: on-&gt;off off-&gt;on). Zippy wants to turn on all the lights. Please help him to solve the puzzle.</p>
<h3>Input</h3>
<p>First line, n, m.</p>
<p>The following n lines, each line is a m-length string, represting the original state. (0 means on and 1 means off)</p>
<p>1&lt;=n,m&lt;=1000</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 42px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">First line, n, m.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 42px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The following n lines, each line is a m-length string, represting the original state. (0 means on and 1 means off)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 42px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1&lt;=n,m&lt;=100</div>
<h3>Output</h3>
<p>n lines, each line is a m-length string. It's obvious that if a valid solution exists, there exists a solution that every switch is flipped no more than once. So 1 means the switch is flipped once and 0 means the swtich remains unflipped.&nbsp;</p>
<p>It's guaranteed that there always exists a solution. If there are multiple solutions, output any of them.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 3
010
010

<strong>Output:</strong>
010
101<span style="white-space: normal;">
</span></pre>