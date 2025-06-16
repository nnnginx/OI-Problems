<p>The hard working ants have built a town called Ant Town. They modeled their town after Manhattan, with H horizontal and V vertical streets which cross in V¡ÁO intersections. As ants don't like water, with the first raindrops comes chaos in Ant Town. Town authorities have placed umbrellas under which any number of ants can hide, but only on N intersections.</p>
<p>When the rain starts, each ant on an intersection starts running, <strong>using streets</strong>, to the nearest intersection with an umbrella. But, if an ant can choose from more than one such intersection, it panics and, not knowing where to go, <strong>stays on its starting intersection</strong> and gets wet. Town authorities use the name "wet intersections" for such starting intersections.</p>
<p>For example, if Ant Town has 10 horizontal and 10 vertical streets, and if there are 4 intersections with umbrellas, then the question marks in the figure represent "wet intersections":</p>
<p style="text-align: center;"><img src="../../../content/stjepang:mravograd.png" alt="" width="305" height="257"></p>
<p><img src="../../embed/stjepang:mravograd.png" alt=""></p>
<p style="text-align: center;"><em>Picture represents first example. We count streets from left to right from 1 to V and from down upwards from 1 to H.</em></p>
<p>Write a program which, given the locations of intersections with umbrellas, determines the <strong>number of "wet intersections</strong>" in Ant Town.</p>
<h3>Input</h3>
<p>The first line contains two integers H and V (1 ¡Ü H, V ¡Ü 30 000), the numbers of horizontal and vertical streets in Ant Town.</p>
<p>Horizontal streets are numbered 1 to H, vertical streets 1 to V.</p>
<p>The second line contains an integer N (1 ¡Ü N ¡Ü 10), the number of intersections with umbrellas.</p>
<p>Each of the following N lines contains two integer h and v, meaning that there is an umbrella on the crossing of horizontal street h and vertical street v. The locations of all umbrellas will be distinct.</p>
<h3>Output</h3>
<p>Output the number of "wet intersections" in Ant Town.</p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br>10 10<br>4<br>4 4<br>4 6<br>6 4<br>9 9<br><br><strong>Output:</strong><br>19<br><strong><br><br>Input:</strong><br>9 9<br>3<br>2 2<br>5 5<br>8 8<br><br><strong>Output:</strong><br>36<br><strong><br><br>Input:</strong><br>100 100<br>2<br>50 50<br>50 51<br><br><strong>Output:</strong><br>0<br></pre>