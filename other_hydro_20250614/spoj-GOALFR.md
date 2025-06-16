<h1>Goal for Ra¨²l</h1>
<p>What would a Madrid programming contest be without some task about Real Madrid? It's a team with a marvellous history of records. For example, the team's topscorer Ra¨²l Gonz¨¢lez has scored 318 goals so far (in 704 games). In this task you are going to help Ra¨²l shoot his 319th.<br><br>Consider a game between Real Madrid and FC Barcelona. The match is in a critical situation: 10 seconds before the end, the score is 3:3 and Ra¨²l has the opportunity of a direct free kick. The question you have to answer is: Is it possible for Ra¨²l to score a goal by kicking the ball in a straight line?<br><br>To model a soccer game, think of the pitch as a rectangle in a coordinate grid, aligned to the axes. The pitch is centred at (0, 0). It is 105m long and 68m wide, thus x ¡Ê [-52.5, +52.5] and y ¡Ê [-34, +34]. The goal is 7.32m long and centred on the short side of the field. The coordinates of the four goal posts are thus (¡À52.5, ¡À3.66). Real Madrid is on the left side and has to shoot the ball into the right goal (where x&gt;0).<br><br>To simplify things a bit, we think of the ball and the goal posts as points in space without any volume. Players, on the other hand, have an action radius, i.e. the maximum distance from their position where they can still reach the ball.</p>
<h3>Input</h3>
<p>The input consists of several test cases. The first line of the input file contains one integer N, the number of cases that follow.<br><br>Each test case starts with a blank line. Then follow the x and y coordinates of the ball. The third line contains the x coordinate, y coordinate and action radius of the FC Barcelona Goalkeeper.<br><br>Have a look at the images and the corresponding sample input given:</p>
<table border="0" align="center">
<tbody>
<tr>
<th scope="col">Sample input 1</th><th scope="col">Sample input 2</th>
</tr>
<tr>
<td><img title="Sample input 1: Goal!" src="../../../content/jbw:goal_for_raul_1.png" alt="Sample input 1: Goal!" width="150" height="89"></td>
<td><img title="Sample input 2: no Goal" src="./22620/file/hKggUDVc.png" alt="Sample input 2: no Goal" width="150" height="87"></td>
</tr>
<tr>
<td>Goal</td>
<td>No Goal</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a line containing one of the following words:<br><br>"Goal!" if it is possible to shoot the ball in a straight line into the goal, without the goalkeeper intercepting it.<br><br>"No goal..." if it is not possible to do so.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br><br>15.0 -20.0<br>42.5 2.0 5.0<br><br>20.0 11.0<br>34.0 6.0 5.0<br><br><strong>Output:</strong><br>Goal!<br>No goal...<br></pre>