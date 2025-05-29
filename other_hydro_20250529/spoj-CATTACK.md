<p>At our soccer training camp, we have rehearsed a lot of motion sequences. In case we are defending, all players except the two strikers of our team are in our half. As soon as we are getting the ball, we are starting a counterattack with a long-range pass to one of our strikers. They know each others motion sequences and may pass the ball to the other striker at fixed points.</p>
<p>There are a lot of decisions: the defender has to select the striker to pass the ball to, and the ball possessing striker has to decide at each of the <em>n</em> fixed points if to pass to the other striker or to run and to dribble. At the last position in the motion sequence of a striker he shoots on the goal. Each of the four actions (long-range pass, dribble, pass, and shoot on the goal) may fail (e.g.  because of a defending player of the opposite team) - so our coach has assigned difficulties.</p>
<p>What is the minimal difficulty of a goal assuming your team plays optimally?</p>
<p align="center"><img src="../../../content/ak15:counterattack.png" alt="example image" width="50%" height="50%"></p>
<p>In the example depicted in the picture, the defending player (cross in left half) passes the ball to one of the strikers (crosses in right half). The strikers move along fixed paths simultaneously. At each of the fixed positions (circles), the ball possessing striker either dribbles with the ball or passes to the other striker. At the last position, he shoots on the goal.</p>
<h3>Input</h3>
<p>The first line of the input consists of the number of test cases <em>c</em> that follow (<em>1 �� c �� 100</em>). Each test case consists of five lines. The first line of each test case contains <em>n</em> (<em>2 �� n �� 100000</em>), the number of fixed points in each strikers motion sequence. It is followed by <em>l<sub>0</sub></em>, <em>l<sub>1</sub></em>, <em>s<sub>0</sub></em> and <em>s<sub>1</sub></em>, the difficulty of a long-range pass to the corresponding striker and the difficulties of the shoots of the strikers. Each striker is described in two lines (first striker <em>0</em>, then striker <em>1</em>): The first line contains <em>n-1</em> difficulties, where the <em>i</em>th number stands for passing from point <em>i</em> to the other player at point <em>i + 1</em>. The second line also contains <em>n-1</em> difficulties, where the <em>i</em>th number stands for dribbling from point <em>i</em> to point <em>i+1</em>. You may safely assume that each difficulty is a non-negative integer less than <em>1000</em>.</p>
<h3>Output</h3>
<p>For each test case in the input, print one line containing the minimal difficulty of a move sequence leading to a goal.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3 5 7 999
9 13
60 5
22 6
5 5
5 3 5 7 999
9 13 8 4
60 5 17 13
22 6 15 11
5 5 18 29

<strong>Output:</strong>
23
42
</pre>