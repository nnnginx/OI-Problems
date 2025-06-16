<p style="text-align: center;"><strong><span style="font-size: medium;">Happy Valentine Day!</span></strong></p>
<p style="text-align: center;"><img title="VMaze" src="../../content/tjandra:Heart_Maze.gif" alt="Valentine Maze" width="300" height="333"></p>
<p style="text-align: center;"><span style="font-size: xx-small;"><span style="font-family: 'andale mono', times;">Picture Source: <a title="VMaze Source" href="http://www.printactivities.com/Mazes/Shape_Mazes/Heart_Maze.html" target="_blank">http://www.printactivities.com/Mazes/Shape_Mazes/Heart_Maze.html</a></span></span></p>
<p>In this valentine day, I'm very happy to know that many SPOJ user happy to help me on my old Valentine Maze Game (2 years ago). I can't imagine what happen if no one guide me in the maze to meet her (my love), of course it will be much worse, because I can lost in the maze for long time. Now, can you help me again to compute what is expected time needed to meet her in the maze if I just walk uniform randomly on all possible dirrection without any guide? I will be very grateful for your help.</p>
<p>For simplicity, there will be no Chocolate in the map, of course I have collected all the chocolates this valentine&nbsp;<img title="Cool" src="../../gfx/jscripts/tiny_mce/plugins/emotions/img/smiley-cool.gif" border="0" alt="Cool">.</p>
<p>Given a map size <strong>m</strong>��<strong>n</strong>, containing 4 possible elements:</p>
<p><strong>'.'</strong> denoting road (I can walk on this area)</p>
<p><strong>'#'</strong> denoting wall (I can't walk on this area)</p>
<p><strong>'T'</strong> denoting my position (Tjandra) at start (time 0), only appear once on the map.</p>
<p><strong>'W'</strong> denoting Woman I want to meet (Destination), only appear once on the map.</p>
<p>Tjandra always walk one valid step left, right, up or down for each unit of time with equal probability on which direction. Valid step means I still inside the maze and not walk to the wall, I never stop until I arrive on my destination.&nbsp;</p>
<h3>Input</h3>
<p>On the first line, there is an integer <strong>t</strong> denoting number of test cases. Number of test case will be less than or equal to 250.</p>
<p>For each test case:</p>
<p>the first one there are two integers&nbsp;<strong>m</strong>&nbsp;and&nbsp;<strong>n</strong> denoting size of map. <strong>m</strong> and <strong>n</strong>&nbsp;will be less than or equal to 50.</p>
<p>Next <strong>m</strong> line(s) there are <strong>n</strong> characters, each character is element of map that has been described above.</p>
<h3>Output</h3>
<p>For each test case, output expected time required for me to meet her if I just walk uniform randomly on all possible dirrection. Your answer are considered correct if <strong>absolute error</strong> with judge (my) solution is <strong>less than 10<sup>-5</sup></strong>. It's guaranteed that my solution has absolute difference less than 10<sup>-19</sup> with exact answer. If it's impossible for me to reach destination, output "<span style="text-decoration: underline;">Mission Failed!</span>" without quotes.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>8</pre>
<pre>1 3</pre>
<pre>T.W</pre>
<pre>1 3</pre>
<pre>.TW</pre>
<pre>1 4</pre>
<pre>.T.W</pre>
<pre>3 3</pre>
<pre>T..<br>.#.<br>..W</pre>
<pre>3 3</pre>
<pre>T.#<br>...<br>#.W</pre>
<pre>3 3</pre>
<pre>T.#<br>.#.<br>#.W</pre>
<pre>3 3</pre>
<pre>T..<br>...<br>..W</pre>
<pre>5 5</pre>
<pre>##T##<br>.#.#.<br>.....<br>.#.#.<br>##W##</pre>
<pre><strong>Output:</strong></pre>
<pre>4.000000000000</pre>
<pre>3.000000000000</pre>
<pre>8.000000000000</pre>
<pre>16.000000000000</pre>
<pre>16.000000000000</pre>
<pre>Mission Failed!</pre>
<pre>18.000000000000</pre>
<pre>48.000000000000</pre>
<h3>Explanation</h3>
<p>On first test case at time 0, I have one choice: walk right, at time 1 the map will be ".TW" I have two choice , walk right or left with equal probability 0.5 vs 0.5. If I walk right then my mission is completed, so there are 0.5 (50%) chance that I completed my mission at time 2. If I walk left, at time 2 the map will be back to first "T.W" I have one choice again (walk right), at time 3 the map will be ".TW" I have two choice again with equal probability. If I walk right then my mission is completed, so there are 0.5*0.5=0.25 (25%) chance that I completed my mission at time 4. By continuing, we get the series:</p>
<p>2 step with (1/2) chance</p>
<p>4 step with (1/4) chance</p>
<p>6 step with (1/8) chance</p>
<p>...</p>
<p>the answer (expected time) will be 2*1/2+4*1/4+6*1/8+8*1/16+... this series will converge to 4.</p>
<p>&nbsp;</p>
<p>On second test case, initial map is equal to first case at time 1, so the expected time will be 1 unit less than first case. The expected time = 4 - 1 = 3.</p>
<p>&nbsp;</p>
<p><span style="color: #339966;"><span style="color: #339966;"><strong><span style="text-decoration: underline;">Time Limit ��&nbsp;2.5*(My Program Speed, without applying any optimization trick)</span></strong></span></span></p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>