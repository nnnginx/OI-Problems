<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">When relay towers for mobile telephones communicate with the mobile phones in their area, there is</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">always the possibility of interference. So, when assigning the transmission frequency, the FCC makes</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">sure that nearby towers have frequencies that aren't too close. On the other hand, the FCC does not</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">want to assign too many different frequencies; they want to save as many as possible for other uses.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your job is to find an optimal assignment of frequencies.</div>
<p>When relay towers for mobile telephones communicate with the mobile phones in their area, there is</p>
<p>always the possibility of interference. So, when assigning the transmission frequency, the FCC makes</p>
<p>sure that nearby towers have frequencies that aren't too close. On the other hand, the FCC does not</p>
<p>want to assign too many different frequencies; they want to save as many as possible for other uses.</p>
<p>Your job is to find an optimal assignment of frequencies.</p>
<p><img src="file://oI8TXvVi.png" alt="Graph" width="609" height="225"></p>
<p>In this problem, the frequencies will be integers. Nearby towers must be assigned frequencies that differ</p>
<p>by at least 2. You'll find an assignment using as few frequencies as possible. For example, consider the</p>
<p>following two arrangements of towers. Two towers near each other are indicated by the connecting line.</p>
<p>Note that the following are legal frequency assignments to these two tower configurations. However,</p>
<p>the second arrangement does not use the fewest number of frequencies possible, since the tower with</p>
<p>frequency 5 could have frequency 1.</p>
<p><img src="file://p0KTzR4a.png" alt="Frequencies Labelled" width="612" height="233"></p>
<h3>Input</h3>
<p>There will be multiple test cases. Input for each test case will consist of two lines: the first line will</p>
<p>contain the integer n, indicating the number of towers. The next line will be of the form x1 y1 x2 y2 ...</p>
<p>xn yn where xi yi are the coordinates of tower i. A pair of towers are considered "near" each other</p>
<p>if the distance between them is no more than 20. There will be no more than 12 towers and no tower</p>
<p>will have more than 4 towers near it. A value of n = 0 indicates end of input.</p>
<h3>Output</h3>
<p>For each test case, you should print one line in the format:</p>
<p>The towers in case n can be covered in f frequencies.</p>
<p>where you determine the value for f. The case numbers, n, will start at 1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
0 0 5 7.5 1 -3 10.75 -20.1 12.01 -22
6
0 1 19 0 38 1 38 21 19 22 0 21
0

<strong>Output:</strong>
The towers in case 1 can be covered in 3 frequencies.
The towers in case 2 can be covered in 2 frequencies.<span style="white-space: normal;">
</span></pre>