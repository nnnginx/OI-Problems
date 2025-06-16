<p>Mr. Green has a large portion of land divided into square units that are either field or lake areas.<br>He wants to fence a rectangular portion of his lands to use for livestock.<br>The lake areas have a very soft soil and any fence built near those areas have a chance to fall (and<br>then the animals could escape), so no fence should be built near a lake area.</p>
<p><img src="./22660/file/rvNJ8yU1.png" alt="Green's Land" width="565" height="275"></p>
<p>Mr. Green wants to know of how many ways he can fence a rectangular area of his lands without<br>any portion of the fence having a common border with a lake area.<br>In the example above, for a 3x3 land with a lake area in the center, we have 5 possibilities of fence.</p>
<h3>Input</h3>
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:<br>One line with a integer N (1 ≤ N ≤ 300): the size of the land (N xN ).<br>N lines, each with N characters. Each character is either ‘.’ or ‘X’. The j − th character on the<br>i − th line is a ‘X’ if position (i, j) is a lake area, and ‘.’ if it is a field area.</p>
<h3>Output</h3>
<p>For each test case output a line with the number of different valid ways wich Mr. Green can fence his<br>lands.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>3<br>...<br>.X.<br>...<br>3<br>X..<br>...<br>X..<br>6<br>......<br>......<br>......<br>......<br>......<br>......<br>5<br>.....<br>....X<br>.X...<br>.....<br>...XX<br>

<strong>Output:</strong>
5<br>8<br>441<br>23
</pre>