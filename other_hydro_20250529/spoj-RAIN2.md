<p>Country M is pluvian. In City P, it rains frequently and many people complain that they always have trouble crossing the streets when raining. To make people cross the streets easier, the government set many "Automatic Umbrellas" above every crosswalk, shown in the picture below.</p>
<img src="/content/john_jones:rain21.jpg">
<p>Each of these "Automatic Umbrellas" looks like a rectangle board, and their thickless is approximate zero. They can sop up the rain instantly. They are left unused when it's not raining and shuttle from one side to another in the same speed otherwise. The walkers will not be wringing-wet if he walks under the umbrella when it's raining.</p>
<p>When many people want to cross the street, one "Automatic Umbrella" is not enough obviously. The government set many "Automatic Umbrella" on some main crosswalks. The width of each of the "Automatic Umbrella" equals to the width of the crosswalk, and any two of these umbrellas have different height.Their length and speed may be different.</p>
<p>You are to write a program to calculate the total volume of the rain falling to the ground from the time when it starts to rain to T seconds later.</p>
<h3>Input</h3>
<p>The very first line comes a single integer Q, the number of test cases.Q blocks follow.</p>
<p>For each test case:</p>
<p>The first line contains 4 space-separated integers N(&lt;=10), W(&lt;=100), T(&lt;=100), V(&lt;=50), the number of "Automatic Umbrella", the length of the crosswalk in meters, the total time in seconds and the volume of rain falling to the ground per square meter per second.</p>
<p>To simplify the description, we can build a Cartesian coordinate system in the following way: let the left side of the street be the origin, the street be the positive Ox-axes, and the vertical line to the ground be the positive Oy-axes,see the picture below.</p>
<img src="/content/john_jones:rain22.jpg">
<p>Each of the next N lines contains 3 integers xi, li, vi, the initial position(in meter), the length(in meter), the speed(in meter per second) of the i-th umbrella. If vi&gt;0, the umbrella moves to the right side initially; if vi&lt;0, the umbrella moves to the left side initially;if vi=0, the umbrella doesn't move at all.</p>
<p>You can assume that the width of the umbrella and the crosswalk is 1 meter, the rain falls vertically, the speed of the rain will not change and the umbrellas and the crosswalk are absolutely horizontal.</p>
<h3>Output</h3>
<p>For each test case, you should output a single real number(rounded to 2 decimal places) - the answer.You can assume the total distance of all the umbrella's movement will not exceed 550*W.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
2 4 3 10
0 1 1
3 1 -1

<b>Output:</b>
65.00
</pre>