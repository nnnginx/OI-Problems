<p>The XYZ TV channel is developing again a new game show, where a contestant has to make a<br>choice in order to get a prize. The game consists of a triangular stack of balls, each of them having an<br>integer value, as the following example shows:</p>
<p><img src="../../../../../../content/simes:BALLSAG.png"></p>
<p>The contestant must choose exactly one ball and his prize is the sum of the value of that ball and<br>the balls directly on top of it. Notice that the prize can be negative!<br>Your friend is going to participate on the game show, and he wants you to develop a program that<br>can tell the maximum prize possible.</p>
<h3>Input</h3>
<p>Each test case is described using several lines. The first line contains an integer N representing<br>the number of rows of the stack ( 0 &lt; N &lt; 1001). The i-th of the next N lines contains i integers Bij ( -<br>1000 &lt;= Bij &lt;= 1000 for 1 &lt;= j &lt;= i &lt;= N); the number Bij is the value of the j-th ball in the i-th row of<br>the stack (the first row is the topmost one, and within each row the first ball if the leftmost one). After<br>each test case there is a blank line.<br>The last test case is followed by a line containing one zero.</p>
<h3>Output</h3>
<p>For each test case output a line with an integer representing the maximum prize a contestant can<br>make from the stack.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>-2<br>1 -10<br><br>3<br>1<br>-5 3<br>6 -4 1<br>0<br><br><strong>Output:</strong>
-1<br>5<br><br>Note:<br>On the first test case, the optimal solution is to take the ball with value 1, making you remove the ball<br>with value -2, resulting in -1.<br>On the second test case the best option is to take the ball with value 1 on the bottom row, resulting in<br>1+3+1 = 5. </pre>