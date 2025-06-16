<p>Recently Zippy received a puzzle. It is an n*m matrix. In most cells of the matrix, there is a light with a switch. However, some cells do not contain a light with a switch, and they are called "blocks". Once he flips the switch in a cell, lights in visible cells from it(including itself) change to its opposite state (which means: on-&gt;off off-&gt;on). One cell is visible from another, iff they are in the same row or the same column, and there aren't any blocks between them (and of course the two cells should not be blocks). Zippy wants to turn on all the lights. Please help him to solve the puzzle.</p>
<h3>Input</h3>
<p>First line, n, m.</p>
<p>The following n lines, each line is a m-length string, represting the original state. (0 means on, 1 means off and 2 means a block)</p>
<p>1&lt;=n,m&lt;=300</p>
<p>number of blocks&lt;=max(n,m)</p>
<h3>Output</h3>
<p>n lines, each line is a m-length string. It's obvious that if a valid solution exists, there exists a solution that every switch is flipped no more than once. So 1 means the switch is flipped once and 0 means the swtich remains unflipped. Of course, a block do not contain a swtich, so for the cell, you should always output 0.&nbsp;</p>
<p>It's guaranteed that there always exists a solution. If there are multiple solutions, output any of them.&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Firsline, n, m.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 160px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The following n lines, each line is a m-length string, represting the original state. (0 means on, 1 means off and 2 means a block</div>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
2 3
011
121

<strong>Output:</strong>
001
100<span style="white-space: normal;">
</span></pre>