<p>It is well known that programmers enjoy bowling. Bowling is a competitive sport in which a player (the ��bowler��) rolls a bowling ball down a wooden or synthetic lane with the objective of scoring points by knocking down as many pins as possible.<br><br>
For a beginner, scoring is probably the part of bowling which people find hard to understand. Fortunately, but it is not as hard as it seems.<br><br>
As most bowling centers have a scoring computer, you do not usually have to score yourself. I am sure that this makes people lazy and there are probably some regular bowlers who would not be able to score manually if they had to. One day, when it all breaks down, or you are needed to correct a mistake (yes, computers do make mistakes sometimes), an understanding of the scoring rules are necessary.<br><br>
The most difficult part of bowling scoring to comprehend is when a strike or spare is scored, as the score on the scorecard does not get updated immediately.<br><br>
A game consists of ten frames, which start with a full rack of ten pins. In each frame, you have two deliveries of your ball, in which to knock down as many of the ten pins as you can.<br><br>
If you knock down all the pins on your first ball, it is called a strike. The score doesn't get added on straight away because for a strike, you get the values of your next two balls as a bonus. For example, if you score a strike in the first frame, then an 7 and 1 in the second frame, you would score 18 (10+7+1) for the first frame, and 8 for the second frame, making a total of 26 after two frames.
If you knock down some of the pins on the first ball, and knocked down the remainder of the pins in the second ball, it is known as a spare. Again, the score doesn't get added on straight away because for a spare, you get the values of your next ball as a bonus. For example, you if score a spare in the first frame, say an 6 and a 4, then got an 8 and a 1 in the second frame, you would score 18 (6+4+8) for the first frame, and 9 for the second frame, making a total of 27 after two frames.<br><br>
When it comes to the final frame, it is slightly different. In the final frame, you get bonus balls if you strike or spare, to a maximum of three deliveries. If you strike in the first delivery you have the opportunity to strike in the remaining two and have three deliveries in total. If you scored strikes in each of your final three deliveries, the score for the final frame would be 30 (10+10+10). If you spare the final frame, you get the third delivery as a bonus. So, a spare, 9 and 1, followed by a strike would equal 20 (9+1+10).<br><br>
You have to write a program which will calculate the score the player gets for the game given the information about the pins knocked down after each delivery of the ball.


</p><h3>Input</h3>
<p>The first line of the input contains number t &lt;= 1000 �C the amount of test cases. Then the description of each of t test cases follow one per line. Each test case consists of several integers 0 &lt;= a &lt;= 10 �C the amount of pins knocked down after each delivery of the ball. Each test case describes a full game for one player. All the games in the input file are correct.

</p><h3>Output</h3>
<p>For each test case output the number of points the player gets in a game on a separate line.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
10 10 10 10 10 10 10 10 10 10 10 10
3 5 1 5 7 1 10 1 6 10 6 2 1 2 0 5 8 1
9 1 5 0 3 0 8 1 6 4 7 2 7 1 6 3 10 4 4

<b>Output:</b>
300
89
101

</pre>