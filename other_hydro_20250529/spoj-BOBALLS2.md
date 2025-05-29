<p>"Behold, my queen", said the jester, "the great Bouncing Ball Bowl!" The queen boredly waved her hand and sarcastically replied: "Let the fun begin!". And the fun begun! The jester spoke a magic word and all the colorful balls in his bowl started to roll and bounce, creating interesting pictures.</p>
<p>The queen watched vividly for a few minutes, but then she started to be bored again. "Just wait a moment, Your Majesty, in a minute they'll��" started the jester, but the queen interrupted: "I'm a queen! I don't want to wait! Can't you just fast forward it or something?"</p>
<h3>Problem specification</h3>
<p>The jester's box is an <em>X</em> * <em>Y</em> (1&lt;= <em>X</em>, <em>Y</em> &lt;=5000)rectangle. The rectangle contains <em>N</em>(<em>N</em> &lt;=3001) small balls. At any moment, each ball is travelling at the same speed in one of the four diagonal directions.</p>
<p>The movement of the balls is continuous and for the purpose of this problem we may consider them to be points. When two or more balls meet, they bounce in a way described below.</p>
<p>Your task is to determine the state of the box at given moments in time.</p>
<h3>Bouncing specification</h3>
<p>Bouncing does not change the speed of the balls. Following images show how the balls bounce off each other, and also off walls. Each image can be rotated arbitrarily. For example, the first image shows that whenever two balls meet at a right angle, they bounce and depart at a right angle again. One particularly tricky case is shown in the third image.</p>
<p><img src="./21589/file/6Nf0vqBb.png" alt=""></p>
<h3>Input specification</h3>
<p>The input starts with a line containing the dimensions <em>X</em> and <em>Y</em> of the box. We will use a coordinate system with axes parallel to the sides of the box, (0,0) at one of the corners and (<em>X</em>,<em>Y</em>) at the opposite corner.</p>
<p>The second line contains the number of balls <em>N</em>.</p>
<p>Each of the next <em>N</em> lines contains four integers x,y,vx,vy, where (x,y) are the coordinates of one ball at time 0 and (vx,vy) is its current velocity vector. (Each ball will be strictly inside the box and for each ball both the absolute values of vx and vy will be equal to 1. No two balls will start at the same place.)</p>
<p>The following line contains the number of queen's requests M.(1&lt;= M &lt;=20)</p>
<p>On the last line there are M numbers t<sub>1</sub>,��,t<sub>M</sub> �C the points in time the queen wants to see. These numbers will be less than 10<sup>12</sup>.</p>
<h3>Output specification</h3>
<p>As a solution to this problem, we expect a file with M blocks, with the i-th block describing the situation at time t<sub>i</sub>.</p>
<p>Each block must contain N lines, and each line must contain the x and y coordinates of one ball. The balls in each block must be sorted �C primarily by to their first, secondarily by their second coordinate at that point in time.</p>
<p>You may output an empty line between the blocks.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 4
4
1 2 1 1
5 2 1 1
2 1 1 -1
3 1 -1 -1
1
4

<strong>Output:</strong>
1 3
3 2
5 2
6 3
</pre>
<p>Note that the balls that start at (2,1) and (3,1) bounce off each other at a non-integer point in time.</p>