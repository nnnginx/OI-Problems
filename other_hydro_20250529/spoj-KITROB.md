<p>Robots are becoming more and more popular. They are used nowadays not only in manufacturing plants,&nbsp;but also at home. One programmer with his friends decided to create their own home robot. As you may&nbsp;know most programmers like to drink beer when they gather together for a party. After the party there&nbsp;are a lot of empty bottles left on the table. So, it was decided to program robot to collect empty bottles&nbsp;from the table.</p>
<p>The table is a rectangle with the length l and width w. Robot starts at the point (x<sub>r</sub>, y<sub>r</sub>) and n bottles&nbsp;are located at points (x<sub>i</sub>, y<sub>i</sub>) for i = 1, 2, ..., n. To collect a bottle robot must move to the point where&nbsp;the bottle is located, take it, and then bring to some point on the border of the table to dispose it. Robot&nbsp;can hold only one bottle at the moment and for simplicity of the control program it is allowed to release&nbsp;bottle only at the border of the table.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="Example" src="../../content/fidels:KITROB.png" alt="Example" width="141" height="179"></p>
<p>&nbsp;</p>
<p>You can assume that sizes of robot and bottles are negligibly small (robot and bottles are points), so the&nbsp;robot holding a bottle is allowed to move through the point where another bottle is located.&nbsp;One of the subroutines of the robot control program is the route planning. You are to write the program&nbsp;to determine the minimal length of robot route needed to collect all the bottles from the table.</p>
<p>&nbsp;</p>
<p><strong>Input</strong></p>
<p>The first line of the input file contains T, the number of test cases. T test cases follow.</p>
<p>The first line of each test case contains two integer numbers w and l ¡ª the width and the length of the&nbsp;table (2 ¡Ü w, l ¡Ü 1000).</p>
<p>The second line contains an integer number n ¡ª the number of bottles on the table&nbsp;(1 ¡Ü n ¡Ü 18). Each of the following n lines contains two integer numbers x<sub>i</sub> and y<sub>i</sub> ¡ª coordinates&nbsp;of the i-th bottle (0 &lt; x<sub>i</sub> &lt; w; 0 &lt; y<sub>i</sub> &lt; l). No two bottles are located at the same point.</p>
<p>The last line of the test case contains two integer numbers x<sub>r</sub> and y<sub>r</sub> ¡ª coordinates of the robot¡¯s initial&nbsp;position (0 &lt; x<sub>r</sub> &lt; w; 0 &lt; y<sub>r</sub> &lt; l). Robot is not located at the same point with a bottle.</p>
<p>&nbsp;</p>
<p><strong>Output</strong></p>
<p>For each test case, output the length of the shortest route of the robot. Your answer should be accurate within an absolute&nbsp;error of 10<sup>-6</sup>.</p>
<p>&nbsp;</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
1
3 4
2
1 1
2 3
2 1

<strong>Output:</strong>
5.60555127546399<span style="white-space: normal;">
</span></pre>