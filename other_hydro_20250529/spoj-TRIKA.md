<p>
Abotrika is a famous player who plays in a good team. His team is going to play the final match next week and he have to train hard because all his fans are expecting that Abotrika will score more than one goal, so his team-mates suggested helping him in training given that Abotrika will play alone against all his friends in the training.
</p>

<h3>Input</h3>
<p>Given two integers N,M (length and width of the training court) 2 &lt;= N, M &lt;= 20 and X,Y the starting point of Abotrika on the court where X is number of row and Y is number of column 1 &lt;= X &lt;= N, 1 &lt;= Y &lt;= M then P[i][j], where P is the power of each of his friends 0 &lt; P[i][j] &lt;100, and P[X][Y] is the power of Abotrika.
</p>

<h3>Output</h3>
<p>The output must be one line either "<tt>N</tt>" or "<tt>Y</tt>" then the maximum power "Abotrika can get when he pass from his friends to reach the (the goal who is at the cell P[N][M] in the court ). </p>

<p><b>NOTE</b>:  Abotrika's power decreases by the power of his team-mate whom Aboutrika succeeded<strong><em> </em></strong>to get through on his way to score a goal. "<tt>Y</tt>" means that he had scored a goal with power at least 0  and "<tt>N</tt>" if he couldn't reach the goal with zero power at least. Also, Abotrika can only move in two directions -- right and down -- to reach the goal. </p>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 4
1 1
100 55 10 2
20 10 90 1
60 20 22 4
1 30 70 5

<strong>Output:</strong>
Y 23</pre>

<p><b>Explanation</b>: The maximum power Abotrika can get after reaching goal : 100 - (55+10+2+1+4+5) = 23 </p>

<pre><strong>Input:</strong>
2 2
1 1
1 55
20 10

<strong>Output:</strong>
N</pre>

<p><b>Explanation</b>: The maximum power Abotrika can get after reaching goal : 1 - (20+10) = -29 so it will be N.</p>