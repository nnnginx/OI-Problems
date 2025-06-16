<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">In a modernized warehouse, robots are used to fetch the goods. Careful</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">planning is needed to ensure that the robots reach their destinations with-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">out crashing into each other. Of course, all warehouses are rectangular,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and all robots occupy a circular floor space with a diameter of 1 meter.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Assume there are N robots, numbered from 1 through N. You will get to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">know the position and orientation of each robot, and all the instructions,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">which are carefully (and mindlessly) followed by the robots. Instructions</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">are processed in the order they come. No two robots move simultane-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">ously; a robot always completes its move before the next one starts mov-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">ing.</div>
<p>&nbsp;</p>
<p>In a modernized warehouse, robots are used to fetch the goods. Careful&nbsp;planning is needed to ensure that the robots reach their destinations without crashing into each other. Of course, all warehouses are rectangular,&nbsp;and all robots occupy a circular floor space with a diameter of 1 meter.&nbsp;Assume there are N robots, numbered from 1 through N. You will get to&nbsp;know the position and orientation of each robot, and all the instructions,&nbsp;which are carefully (and mindlessly) followed by the robots. Instructions&nbsp;are processed in the order they come. No two robots move simultaneously; a robot always completes its move before the next one starts moving.</p>
<div>
<div>A robot crashes with a wall if it attempts to move outside the area of&nbsp;the warehouse, and two robots crash with each other if they ever try to&nbsp;occupy the same spot.</div>
</div>
<p>&nbsp;</p>
<p><img src="./21983/file/7K3sQg38.png" alt="" width="450" height="211"></p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input is K, the number of test cases. Each test case starts&nbsp;with one line consisting of two integers, 1 ¡Ü A, B ¡Ü 100, giving the size of&nbsp;the warehouse in meters. A is the length in the EW-direction, and B in the&nbsp;NS-direction.</p>
<div>
<div>The second line contains two integers, 1 ¡Ü N, M ¡Ü 100, denoting the&nbsp;numbers of robots and instructions respectively.</div>
<div>Then follow N lines with two integers, 1 ¡Ü Xi ¡Ü A, 1 ¡Ü Yi ¡Ü B and&nbsp;one letter (N, S, E or W), giving the starting position and direction of each&nbsp;robot, in order from 1 through N. No two robots start at the same position.</div>
<div>
<div>Finally there are M lines, giving the instructions in sequential order.&nbsp;An instruction has the following format:</div>
</div>
</div>
<div>
<div>&lt;robot #&gt; &lt;action&gt; &lt;repeat&gt;</div>
</div>
<div>
<div>Where &lt;action&gt; is one of:</div>
<div>
<ul>
<li>L: turn left 90 degrees,</li>
<li>R: turn right 90 degrees, or</li>
<li>F: move forward one meter,</li>
</ul>
</div>
<p>&nbsp;</p>
<p>and 1 ¡Ü &lt;repeat&gt; ¡Ü 100 is the number of times the robot should perform&nbsp;this single move.</p>
<p>&nbsp;</p>
</div>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output one line for each test case:</p>
<div>
<ul>
<li>Robot i crashes into the wall, if robot i crashes into a wall. (A&nbsp;robot crashes into a wall if Xi = 0, Xi = A + 1, Yi = 0 or Yi = B + 1.)</li>
<li>Robot i crashes into robot j, if robots i and j crash, and i is the&nbsp;moving robot.</li>
<li>OK, if no crashing occurs.</li>
</ul>
</div>
<p>&nbsp;</p>
<p>Only the first crash is to be reported.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
5 4
2 2
1 1 E
5 4 W
1 F 7
2 F 7
5 4
2 4
1 1 E
5 4 W
1 F 3
2 F 1
1 L 1
1 F 3
5 4
2 2
1 1 E
5 4 W
1 L 96
1 F 2
5 4
2 3
1 1 E
5 4 W
1 F 4
1 L 1
1 F 20


<strong>Output:</strong>
Robot 1 crashes into the wall
Robot 1 crashes into robot 2
OK
Robot 1 crashes into robot 2
</pre>