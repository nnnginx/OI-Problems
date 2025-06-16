<p>Bob has unusual problem. In Byteland we can find a lot of hills and cities. King of Byteland ordered Bob to deliver magic balls from one city to another. Unfortunately, Bob has to deliver many magic balls, so walking with them would take too much time for him. Bob came up with great idea - catapulting them.</p>
<p>Byteland is divided into intervals. Each interval contains city and hill.</p>
<p>Bob can catapult magic ball accurately from city A to city B, if between them there isn't higher hill than A's hill.</p>
<h3>Input</h3>
<p>Every test case contains N and M (N&lt;=50000) (M&lt;=50000), number of intervals and number of balls.</p>
<p>In next line there's N numbers H(H&lt;=10^9) separated by one space.</p>
<p>In next M lines numbers A and B (1&lt;=A,B&lt;=N), number of city from which we want to catapult the ball and number of city to which we want to catapult the ball.</p>
<h3>Output</h3>
<p>Write one number - number of magic balls that Bob can catapult successfully.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>7 3<br>2 3 5 4 2 1 6<br>3 5<br>2 5<br>4 6<br><br><strong>Output:</strong><br>2<br><br>Bob can catapult ball number 1 and 3. <br></pre>