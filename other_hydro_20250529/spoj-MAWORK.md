<p>
Every morning you have to drive to your workplace. Unfortunately, roads are under constant repair. Fortunately, administration is aware that this may cause trouble and they enforce a strict rule on roadblocks: roads must be blocked only half of the time. However, contractors are free to schedule their working hours, still they must follow regulations:
</p>
<ul>
<li>Working periods (when the road is blocked) and rest periods (when the road is open) must alternate and be of fixed length.</li>
<li>The beginning of the day (time zero) must coincide with the beginning of a period.</li>
</ul>
<p>
Write a program that, given a description of the road network and of contractors schedules outputs the minimal time needed to drive from home to work.
</p>
<h3>Input</h3>
<p>
The first line of the input contains a number T �� 10 that indicates the number of test cases to follow.
The road network is represented on a N x N grid and the first line of each test case consists in the number N, 2 �� N �� 25. </p>
<p>Then follows N lines of N characters that represent the road network at time zero. Those lines are made of "." (standing for open road) and "*" (standing for roadblock) and they encode the rows of the grid in increasing order, while columns are also presented in increasing order. Conventionally, your home is at the position first row, first column, while your workplace is at the position last row, last column. Furthermore, you leave home at time t=0, that is, your starting position is first row, first column at time zero.</p>
<p>At a given time t, your car must be on some "open road" cell. It takes one time unit to drive to any of the four adjacent cells heading toward north, south, west or east, and you may also choose to stay on the same cell for one time unit. Of course, those five moves are valid if and only if the target cell exists and is free at time t+1.</p>
<p>Finally comes N lines of N characters that represent the contractors schedules. Those lines match the ones of the grid description and are made of N characters 0,1,...,9 that specify the duration of the working (and rest) period for a given cell. Observe that 0 is a bit special, since it means that the corresponding cell status does not change.
</p>
<h3>Output</h3>
<p>
The output consist in a single line for each test case, holding either the requested time, or NO, if driving from home to work is not possible.
</p>
<h3>Example</h3>
<div align="left">
<h4>Input:</h4>
<pre>2
10
.*********
........**
*.******.*
*.******.*
*.******.*
*........*
*.******.*
*.******.*
*........*
********..
0000000000
0000000000
0000000000
0000000000
0000000000
0123456780
0000000000
0000000000
0123456780
0000000000
3
...
**.
**.
021
002
000
</pre>
<h4>Output:</h4>
<pre>34
NO
</pre>
</div>