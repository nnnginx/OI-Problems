<p>A spaceship has been sighted heading towards Earth. For the entire time that humanity has been monitoring it, it has not altered its course, it only changed speed for unknown reasons. As such, all the possible places on Earth where the spaceship might end up landing form a straight line; depending on how much it changes speed, it will land at different times, meaning a different point on this line due to Earth's rotation.</p>
<p><strong>n</strong>&nbsp;people want to be the first to meet the aliens - they picked a point <strong>x</strong><sub><strong>i</strong>&nbsp;</sub>on this line and wait at that point in their vehicle with speed <strong>v<sub>i</sub></strong>. Now they are all anxiously waiting for the spaceship's arrival. NASA has given a list of&nbsp;<strong>q </strong>most likely locations where the spaceship might end up landing - and everyone wants to know who would get to be the first to meet the aliens if the spaceship landed at each of the given points. They turned to you for help!</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>1 ¡Ü n , q ¡Ü 300,000 </strong>- the number of people wishing to meet the aliens and the number of possible points where the spaceship might land.</p>
<p>The following <strong>n</strong>&nbsp;lines contain two integers <strong>0 ¡Ü x<sub>i</sub>&nbsp;&lt; 10<sup>9 </sup>&nbsp;</strong>and <strong>0 &lt; v<sub>i </sub>¡Ü 10<sup>9</sup>&nbsp;</strong>- the point on the line where the <strong>i</strong>-th person is waiting and the speed of his vehicle. Additionally, <strong>x<sub>i</sub>&nbsp;</strong><strong>= x</strong><sub><strong>j</strong> </sub><strong>¡ú v</strong><sub><strong>i</strong> </sub><strong>¡Ù v</strong><sub><strong>j</strong></sub>.</p>
<p>The last line contains <strong>q</strong>&nbsp;distinct integers <strong>0 ¡Ü q<sub>i </sub>&lt; 10<sup>9&nbsp;</sup></strong>- the points on the line where the spaceship might end up landing. You may assume the spaceship will not land at any point containing a person waiting in a vehicle.</p>
<h3>Output</h3>
<p>For each query <strong>q<sub>i&nbsp;</sub></strong>output the number of people who will arrive at the spaceship first if it lands at that point. A person at <strong>x</strong><sub><strong>j</strong> </sub>with speed <strong>v</strong><sub><strong>j</strong> </sub>will arrive at <strong>q<sub>i</sub>&nbsp;</strong>in time <strong>|</strong><strong>x</strong><sub><strong>j</strong> </sub><strong>- q</strong><sub><strong>i</strong></sub><strong>| / </strong><strong>v</strong><sub><strong>j</strong></sub>. The people who will arrive at the spaceship first are those <strong>j</strong>&nbsp;for whom the fraction is minimal out of all people. Then, in the same line, output the 1-based indices of these people as they were given in the input, sorted in ascending order.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 7
10 5
30 1
20 4
100 1
5 31 22 15 85 60 61

<strong>Output:</strong>
1 1
1 2
1 3
1 1
2 1 4
2 1 3
1 1</pre>