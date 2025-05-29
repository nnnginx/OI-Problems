<p><span style="font-size: x-large;"><strong>Windy Cannon</strong></span></p>
<p><img src="../../../content/tjandra:A_cover.png" alt=""></p>
<p>This day is very windy, the wind blow very fast that it may be faster than the speed of cannon ball. On this windy day, Gunawan want to test his new prototype cannon, he want to shoot the target at specific location. But before doing that, he wonder how long it take for the cannon ball to hit the target. He know percisely the position of his cannon, the location of the target, the speed of his cannon ball, the speed of wind blows, and the direction of the wind, but unfortunately he forgot to bring the calculator so he ask you for help to calculate the minimum time needed for the cannon ball to hit the target or specify if it's impossible. Can you help him? You can assume that the speed of cannon ball relative to the wind is constant, all other physical effect such as gravity, air friction, temperature, magnus effect are ignored.</p>
<p><span style="font-size: large;"><strong>Input</strong></span></p>
<p>The first line there are 4 integers and 1 character CP, TP, CBS, WS, WD denoting cannon position (m), target position (m), cannon ball speed (m/s), wind speed (m/s), and wind direction respectively.</p>
<p><strong><span style="font-size: large;">Output</span></strong></p>
<p>Print how many seconds the minimum time needed for cannon ball to hit the target rounded to 6 digits after decimal point.</p>
<p>If it's impossible for the cannon ball to hit the target, print "Impossible" without quotes.</p>
<p><strong><span style="font-size: large;">Constraint</span></strong></p>
<p>0 ¡Ü CP ¡Ü 100</p>
<p>0 ¡Ü TP ¡Ü 100</p>
<p>0 ¡Ü CBS ¡Ü 100</p>
<p>0 ¡Ü WS ¡Ü 100</p>
<p>if WD = 'L', it means that the wind blow into negative direction (left in catesian plane).</p>
<p>if WD = 'R' it means that the wind blow into positive direction (right in cartesian plane).</p>
<p><strong><span style="font-size: large;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2 10 2 1 L</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>8.000000</pre>
<p><strong><span style="font-size: large;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2 10 2 1 R</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2.666667</pre>
<p><strong><span style="font-size: large;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2 10 2 3 L</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>Impossible</pre>
<p><strong><span style="font-size: large;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>10 2 2 3 L</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1.600000</pre>
<p><strong><span style="font-size: large;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>50 50 12 34 R</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>0.000000</pre>
<p><strong><span style="font-size: large;">Sample 4 Explanation</span></strong></p>
<p><img src="../../../content/tjandra:A_explain.png" alt=""></p>
<p>The cannon ball move at speed 2 m/s relative to the wind, so if it shoot to the right, because of the wind blowing 3 m/s to the left relative to the ground, the cannon ball move (3-2=1) m/s to the left relative to the ground and will eventually hit the target in 8 seconds, but this is not optimal, it's faster to shoot the cannon ball to the left, because the wind blowing 3 m/s to the left relative to the ground (and the same direction as the cannon ball move relative to the wind), so the cannon ball will move (3+2=5) m/s to the left relative to the ground and will eventually hit the target at (10-2)/5 = 8/5 = 1.6 seconds. We need to print the result rounded to 6 digit after decimal places, so the minimum time needed for the cannon ball to reach the target is 1.600000 seconds.</p>