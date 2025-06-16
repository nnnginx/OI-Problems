<p>In the Middle Ages the capital of Byteland was surrounded by stout walls to protect the citizens from intruders. The gates of the city were well guarded and the drawbridge was lifted for the night, and everyone felt pretty happy and secure. At least, for a while.
</p><p>
With time the usual disadvantages of a walled city became apparent. As the population increased, crime flourished in the cramped living space. Eventually it all became so bad that the mayor decided to intervene. Some of the guards were reassigned from their usual occupation of reading newspapers in the guard posts near the gates, and told to start patrolling the city. Many of the officers were rather unhappy about all this, especially after the first men to go on the beat returned with bleeding noses and bumps on their heads. Sensing the low morale of the men, the Captain of the Guard, a bright young individual, decided to reinterpret the order he had received from the mayor. He decided that patrol officers would only go out in large groups and armed to the teeth, and would only move along a few carefully chosen streets from which they could see everything that was going on in the city without actually getting involved.
</p><p>
The city is laid out on a regular grid, with each street running North-South or East-West from one end of the city to the other (as far as the walls allow). Every point with integer coordinates is at an intersection of two streets, one leading North-South, the other East-West. The walls that surround the city form a simple polygon whose sides run directly alongside sections of some streets of the city.
</p><p>
Every street in the set of 'patrolled streets' chosen by the Captain intersects with at least one other patrolled street. Furthermore, if a point belongs to one of the streets of the city then it is visible from some point of one of the patrolled street (points see each other iff the line segment connecting them is a fragment of a street). Finally, the set of patrolled streets chosen by the Captain consists of the minimum possible number of streets.
</p><p>
Given a description of the capital of Byteland, find out how many of its streets were actually patrolled by guards after the Captain issued his order.

</p><h3>Input</h3>
<p>
The first line of input contains t - the number of test cases. t test cases follow.
</p><p>
For each test case, the first line contains a single integer n - the number of sections the city wall consists of (4 &lt;= n &lt;= 2000). The second line contains exactly n integers a<sub>1</sub>,...,a<sub>n</sub> describing successive sections of wall (1&lt;=|a<sub>i</sub>|&lt;=100000). Any two successive sections of wall are perpendicular to each other. The length of the i-th section is the absolute value of a<sub>i</sub>, while its direction is described by the sign of a<sub>i</sub> (positive means northbound or eastbound, negative - southbound or westbound when traversing the walls clockwise).

</p><h3>Output</h3>
<p>
For each test case output a single integer k - the number of elements of the patrolled set of streets selected by the Captain.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
14
+2 +2 +2 +2 -4 +2 +1 +2 -3 +2 -2 -8 +4 -2

<b>Output:</b>
4
</pre>

<img src="/content/adrian:ofbeat.png" alt="Illustration of the sample test data. Blue lines indicate the set of patrolled streets">