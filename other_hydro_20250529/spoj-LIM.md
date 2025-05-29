<h1>Lost in Madrid</h1>
<p>Programming contests can be very exhausting. After five hours of intensive programming, you want to get some well-deserved rest and make yourself on the way to your hotel. Unfortunately, you don't quite remember the way to get there... but that doesn't matter: In good spirits (due to a successful contest?) you set out.</p>
<p>As you don't know the exact way, you decide to walk around in the following fashion: Start at the contest site (denoted by id&nbsp;0) and choose a street at random. Follow the street to the next intersection, and choose another street at random. Every street at an intersection has the same probability of being chosen. You might even decide to take the street back where you came from. As you're on foot, you can use the streets in both directions, unlike in "Madrid's One Way Streets".</p>
<p>Your walk stops once you encounter your hotel (id&nbsp;=&nbsp;300) or one of the tourist information booths (id&nbsp;&gt;&nbsp;290) where you can ask for the way. You can assume there is at least one path connecting you to either type of object.</p>
<p>Because you don't speak a lot of spanish (apart from some verbs that you can conjugate thanks to problem "Spanish Verbs"), you'd like to know the probability that you arrive at your hotel directly, without first arriving at a tourist information booth.</p>
<h3>Input</h3>
<p>The input consists of several testcases, separated by an empty line.</p>
<p>Each testcase starts with <em>S</em>, the number of streets. The following <em>S</em> lines contain two numbers 0&nbsp;¡Ü&nbsp;<em>A,&nbsp;B</em>&nbsp;¡Ü&nbsp;300 each. This means that there is a street connecting intersection <em>A</em> to intersection <em>B</em>. The same street will not appear multiple times in the input.</p>
<p>The input ends with <em>S</em>=0. This testcase should not be processed.</p>
<h3>Output</h3>
<p>For each testcase, print the probability to arrive directly at the hotel, rounded to three decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>0 291<br>0 292<br>0 300<br><br>2<br>0 300<br>291 300<br><br>2<br>0 291<br>291 300<br><br>7<br>0 292<br>0 88<br>0 14<br>0 300<br>292 88<br>88 300<br>14 300<br><br>0<br><br><strong>Output:</strong><br>0.333<br>1.000<br>0.000<br>0.579<br></pre>