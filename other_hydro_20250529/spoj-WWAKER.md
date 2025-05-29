<p>The world is in danger once again, and Link is the hero who will save us! In order to save the world, Link must travel overseas and collect some legendary items.<br><br>The sea can be described as an infinite 2D plane with a Cartesian coordinate system, in which the point (0,0) denotes the center of the sea. Also, the cardinal directions are defined as usual:</p>
<p style="text-align: center;"><img src="../../../content/reiracofage:ROSA" alt="Cardinal drections" width="250" height="243"></p>
<p><br>Link must use his boat to travel. Unfortunately, Link's boat has a limitation: the boat can only move in the same direction as the Wind. So, for instance, if the wind is blowing North, Link can only travel to the North. If the wind is not blowing at all, Link doesn't move at all, too.</p>
<p>Fortunately, Link has the <em>wind waker</em>, the magical baton. With this baton, Link can conduct the <em>Wind's Requiem</em>, a mystical melody that allows Link to control the wind. Each time the wind waker is used, Link can either make the wind stop blowing (this action is represented by the letter X) or make the wind blow in one of the 8 cardinal directions (North (N), South (S), East (E), West (W), Northeast (NE), Southeast (SE), Southwest (SW), Northwest(NW)).</p>
<p style="text-align: center;"><img src="../../../content/reiracofage:WWAKER" alt="Wind Waker" width="600" height="117"></p>
<p style="text-align: center;">Link using the wind waker</p>
<p><br>Link must go to the position (x<sub>2</sub>,y<sub>2</sub>) and stop there, to collect a legendary item. Right now, Link is at the position (x<sub>1</sub>,y<sub>1</sub>) and the wind is not blowing. You must find a trajectory from (x<sub>1</sub>,y<sub>1</sub>) to (x<sub>2</sub>,y<sub>2</sub>). A trajectory consists of a sequence of uses of the wind waker at certain positions. For example, to go from (0,0) to (1,1), a possible trajectory is:</p>
<ol>
<li>At point (0,0), make the wind blow north;</li>
<li>At point (0,1), make the wind blow east;</li>
<li>At point (1,1), make the wind stop blowing.</li>
</ol>
<p>You must find a trajectory that:</p>
<ul>
<li>Minimizes the number of times Link uses the wind waker;</li>
<li>In case of a tie, minimizes the total distance traveled;</li>
<li>In case of a tie, uses the lexicographically smaller sequence of wind direction changes. Use <em>E &lt; N &lt; NE &lt; NW &lt; S &lt; SE &lt; SW &lt; W &lt; X</em>. For example, a trajectory that changes the wind to N, then to SW, then to W is preferable over a trajectory that changes the wind to N, then to W, then to E, because <em>(N,NW,W)</em> is lexicographically smaller than <em>(N,W,E)</em> (because <em>N=N, NW &lt; W</em>).</li>
</ul>
<p><br>Check the sample input and output.<br><br>Note: The names "Link", "The Wind Waker" and some images above are copyrighted by<strong> Nintendo (r)</strong>.<br>The author just wanted to make the problem more interesting. The author supports <strong>Nintendo</strong>!</p>
<h3>Input</h3>
<p>The input file consists of one or more test cases. Each test case is described by a line containing four integers x<sub>1</sub>, y<sub>1</sub>, x<sub>2</sub>, y<sub>2</sub> (|x<sub>1</sub>|, |y<sub>1</sub>|, |x<sub>2</sub>|, |y<sub>2</sub>|&nbsp;¡Ü 5&nbsp;¡Á 10<sup>4</sup>, (x<sub>1</sub>, y<sub>1</sub>)<sub> ¡Ù</sub> (x<sub>2</sub>, y<sub>2</sub>)).<br><br>The file ends with EOF.</p>
<h3>Output</h3>
<p>For each test case, print a line containing K, the number of times the wind waker is used. In the next K lines print<em> x<sub>i</sub> y<sub>i</sub> D</em>, meaning that the wind waker must be used to change the wind direction to <em>D</em> at the position <em>(x<sub>i</sub>,y<sub>i</sub>)</em>. Print the coordinates rounded to exactly two fractional digits, and use<em> D</em>=<em>'S',N','W','E','SE','SW','NE','NW' </em>or <em>'X'</em>. Print the events in the order they occur in the trajectory.<br><br>After the <em>K</em> lines, print the total distance traveled, rounded to exactly three fractional digits. Print a blank line after each test case. Check the sample output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>0 0 0 1<br>0 0 3 2

<strong>Output:</strong><br>2<br>0.00 0.00 N<br>0.00 1.00 X<br>1.000<br><br>3<br>0.00 0.00 E<br>1.00 0.00 NE<br>3.00 2.00 X<br>3.828<br><br></pre>