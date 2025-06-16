<div align="justify">
<p>
Define <b>r(s)</b> to be the complement of the reverse of the binary string <b>s</b>. i.e. Reverse <b>s</b> and then convert all 1's to 0's and all 0's to 1's. <br>
Further define a sequence of binary string as follow: s<sub>0</sub> = 1 and s<sub>n</sub> = s<sub>n-1</sub>1r(s<sub>n-1</sub>). i.e.<br>
s<sub>0</sub> = 1<br>
s<sub>1</sub> = 110<br>
s<sub>2</sub> = 1101100<br>
s<sub>3</sub> = 110110011100100<br>
...<br>
<br>
We then program a robot to move at a steady speed of 1 unit per second and make a right-angle turn according to the characters of s<sub>10</sub> after every unit of movement. At the kth turn, the robot turns to left if the kth character of s<sub>10</sub> is a 1, and to right otherwise. The figure below shows the whole path of the robot.<br>
<img src="/content/myprasanna:dragoncurves.jpg">
<br>
The robot is placed at the origin (the small circle) and face east originally. It ends up at the coordinates (-32,32) (the small spot) after 2048 seconds. The path of the robot is known as a dragon curve, a pretty well-known pattern of fractal. <br>
<br>
If the robot is now programmed with input string s<sub>30</sub> (with identical initial conditions as above), it will keep moving and then stop after 2<sup>31</sup> seconds. We want to know the location of the robot at any given time.<br>
</p>
<br>

<b>Input Format:</b><br>
Input consists of multiple problem instances. Each instance consists of a single non-negative integer <b>n</b>, where <b>n</b> &lt;= 10<sup>9</sup>. The input data is terminated by a "-1". There will be less than 5000 test cases.<br>
<br>
<b>Output Format:</b><br>
For each input integer <b>n</b>, print out the location of the robot right after <b>n</b> second since the robot starts its journey with input string s<sub>30</sub>. The location should be printed with the format "(x,y)" in a single line.<br>
<br>
<b>Sample Input:</b><br>
<pre>1
2
3
2048
1000000000
-1
</pre><br>
<b>Sample Output:</b><br>
<pre>(1,0)
(1,1)
(0,1)
(-32,32)
(9648,-31504)
</pre>
</div>