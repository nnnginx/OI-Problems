<p>In the kingdom of Thuvax, a mobile game called Thuball became very popular. &nbsp;<br>The description of the game is as follows:<br>A mobile phone made in Thuvax has a screen made of X*Y pixels. Thuball is played by throwing a ball (of size 1 pixel) at an angle of 45 degrees from the bottom of the screen. The ball changes its direction if and only if it hits the left/right/top edge of the screen or an obstacle on its way. &nbsp;<br>There are N fixed obstacles (of size 1 pixel each) on the screen. There are no obstacles in the bottom-most row of the screen. &nbsp;<br>If the moving ball's edge comes in contact with an obstacle's edge, it gets reflected by 90 degrees. <br>If the moving ball's corner comes in contact with an obstacle's corner, it is reflected by 180 degrees. <br>In both reflections the obstacle doesn't move. <br>There is a reflector of length L pixels placed below the bottom row, which reflects (akin to mirror reflection, ie 90 degrees) the ball incident on it. <br>The game finishes only when the ball reaches the bottom row and the reflector is not present below it. The total distance (in pixels) travelled by the ball is the score attained during a round until the game finishes.<br>If the game does not finish, the score is 0.<br> <br>Gosu, a Thuvaxian was very fond this game. He had set the highest score in Thuball in his friend Visu's phone. Not happy with the situation where he didn't have the highest score, Visu decided to recruit you to do his dirty work. <br>Visu is lazy and doesn't want to move the reflector after starting the game. But, he wants to ensure that he gets the highest score possible with a reflector of length L when its kept stationary in any position. <br>Help Visu out by telling him the maximum score he can get without moving the reflector for Q different lengths.<strong></strong></p>
<h3><strong>Input</strong></h3>
<pre>First line contains two integers X and Y, which are the height and width of the screen. (1&lt;=X,Y&lt;=1000)
Second line contains the number of obstacles N followed by N lines with two integers xi and yi, position of each obstacle.
Consider the bottom-left corner of the screen as origin and the top-right corner to have the coordinates:(X-1,Y-1). 
The next line contains Q, for the number of cases (for different lengths of the reflector).(1&lt;=Q&lt;=1000)
Followed by Q lines with one positive integer L, representing the length of the reflector.</pre>
<h3>Output</h3>
<pre>For each query output the maximum score Visu can achieve without moving the reflector in a single line.</pre>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3 4</pre>
<pre>1</pre>
<pre>2 3</pre>
<pre>1</pre>
<pre>3</pre>
<pre><strong>Output:</strong>
6
</pre>