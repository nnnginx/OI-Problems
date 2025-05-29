<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We all know "Connect 4 Game", One day Khairy has a Grid with infinite height and n numbers representing the number of discs in the ith column.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It's guaranteed that no empty cells between any discs in the same column.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for each disc in the grid if Khairy saw a disc on its left OR its right, he'll say "Wal3a".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given the N numbers, What's the maximum number that Khairy will say "Wal3a"!</div>
<p>Khairy is a small guy who likes gold very much, but he has a problem in his eyes and the word "WAL3A" (WAL3A in arabic means "Firing"), whenever he likes something very much sooner or later it is destroyed by any means (Please don't impress him with something you want :|)</p>
<p>One day Khairy visited the National Museum and saw a Grid with infinite height and N columns and each column <em>i</em> contains X<em>i</em> Gold Alloys. No empty cells between Alloys in the same column.</p>
<p>Khairy is a short guy, so he only sees the first row of the grid (High things may survive), also he is only impressed by at least two Gold Alloys adjacent to each other in a row, so if he found an Alloy alone in the row, he ignores it, else he would shout "WAL3AAAAAAAA".</p>
<p>Unfortunately all Gold Alloys that impress Khairy in the 1st row are destroyed and disappeard :S, consequently the Alloys of the same columns above the destroyed Alloys fall to the the cell which is directly below it (each affected column height is decreased by 1 unit). Khairy continues saying "WAL3A" till he finds the first row not impressing anymore.</p>
<p>The example below Khairy would say "WAL3A" twice and 7 gold alloys are destroyed.</p>
<p style="text-align: center;"><img style="vertical-align: middle;" title="Black Blocks are Gold Alloys Destroyed By Khairy" src="file://wDzfGMK8.png" alt="Black Blocks are Gold Alloys Destroyed By Khairy" width="344" height="191"></p>
<p style="text-align: center;">&nbsp;</p>
<p>Of course the museum lost a fotune during Khairy's visit, so could you help the government find how many Gold Alloys are destroyed by Khairy.</p>
<h3>Input</h3>
<p>The first line of input contains an integer&nbsp;<strong>T</strong> (1 &lt;= 20 &lt;= <strong>T</strong>) followed by <strong>T</strong> test cases.</p>
<p>Each test case contains a positive integer&nbsp;<strong>N</strong>&nbsp;[1 &lt;= <strong>N</strong> &lt;= 10<sup>5</sup>] followed by&nbsp;<strong>N</strong> integers [0 &lt;= <strong>X<sub>i</sub></strong>&nbsp;&lt;= 10<sup>9</sup>] separated by spaces (see sample input for more clarification).</p>
<h3>Output</h3>
<p>For each test case output one line contains&nbsp;how many Gold Alloys are destroyed by Khairy.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>1 2 2 1 5<br>3<br>7 7 7

<strong>Output:</strong>
7<br>21&nbsp;</pre>