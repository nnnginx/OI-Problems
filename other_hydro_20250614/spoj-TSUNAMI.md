<p>The country of Cartesia can be described simply by a Cartesian plane. The x-axis is a shoreline. The positive y half-plane is land, and the negative y half-plane is ocean. Several large cities dot the mainland. Their positions can be described by coordinates (x,y), with y&gt;0. Unfortunately, there are sometimes tsunamis in the ocean near Cartesia. When this happens, the entire country can flood. The waters will start at y=0 and advance uniformly in the positive y direction.</p>
<p>Cartesia is trying to develop a tsunami warning system. The warning system consists of two components: a single meteorological center which can detect a tsunami miles out, and wired connections which can carry the warning from city to city in straight lines (No wireless communication!!). Despite the lack of wireless communications, the wired connections can carry the warning virtually instantaneously.</p>
<p>A city is considered safe if it either has the meteorological center, or if it has a direct wire connection to another safe city (i.e. if it has a multi-hop cable path to the single meteorological center).</p>
<p>Unfortunately, a simple engineering problem is made more complicated by politics! If a city A receives the warning from city B, and city B is further away from the shore than city A, then city A¡¯s leaders will complain! ¡°We¡¯re closer to the ocean than city B, so the warning should have gone through us!¡± With a sigh, you agree to find a solution where no city will get the warning from a city that¡¯s further from the shore. (This means that the meteorological center must be in a city that¡¯s closest to the shore.)</p>
<p>Given a description of Cartesia, find the least amount of cable necessary to build a tsunami warning system where every city is safe, and no city will receive the warning from another city that is further from the shore.</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There will be several test cases in the input. Each test case will begin an integer n</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(1¡Ün¡Ü1,000) on its own line, indicating the number of cities. On each of the next n lines</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">will be a pair of integers x and y (-1,000¡Üx¡Ü1,000, 0&lt;y¡Ü1,000), each of which is the (x,y)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">location of a city. These integers will be separated by a single space. Within a test case,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">all (x,y) pairs will be unique. The input will end with a line containing a single 0.</div>
<p>There will be several test cases in the input. Each test case will begin an integer n (1¡Ün¡Ü1,000) on its own line, indicating the number of cities. On each of the next n lines will be a pair of integers x and y (-1,000¡Üx¡Ü1,000, 0&lt;y¡Ü1,000), each of which is the (x,y) location of a city. These integers will be separated by a single space. Within a test case, all (x,y) pairs will be unique. The input will end with a line containing a single 0.</p>
<h3>Output</h3>
<p>For each test case, output a single real number on its own line, which is the minimum amount of cable which must be used to build the tsunami warning system. Output this number with exactly two decimal places. Output no extra spaces, and do not separate answers with blank lines.</p>
<h3>Example Input:</h3>
<pre>3
100 10
300 10
200 110
4
100 10
300 10
200 110
200 60
0</pre>
<h3>Example Output:</h3>
<pre>341.42
361.80</pre>
<p>&nbsp;</p>