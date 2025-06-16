<p>You have recently made a grid traversing robot that can<br> nd its way from the top left corner of a grid to the<br>bottom right corner. However, you had forgotten all your<br>AI programming skills, so you only programmed your robot<br>to go rightwards and downwards (that's after all where the<br>goal is). You have placed your robot on a grid with some<br>obstacles, and you sit and observe. However, after a while<br>you get tired of observing it getting stuck, and ask yourself<br>\How many paths are there from the start position to the<br>goal position?", and \If there are none, could the robot have<br>made it to the goal if it could walk upwards and leftwards?"<br>So you decide to write a program that, given a grid of<br>size n x n with some obstacles marked on it where the robot<br>cannot walk, counts the dierent ways the robot could go<br>from the top left corner s to the bottom right t, and if none,<br>tests if it were possible if it could walk up and left as well.<br>However, your program does not handle very large numbers, so the answer should be<br>given modulo 2^31 - 1.</p>
<h3>Input</h3>
<p>On the rst line is one integer, 1 &lt; n &lt;= 1000. Then follows n lines, each with n characters,<br>where each character is one of '.' and '#', where '.' is to be interpreted as a walkable<br>tile and '#' as a non-walkable tile. There will never be a wall at s, and there will never<br>be a wall at t.</p>
<h3>Output</h3>
<p>Output one line with the number of dierent paths starting in s and ending in t (modulo<br>2^31 - 1) or THE GAME IS A LIE if you cannot go from s to t going only rightwards and<br>downwards but you can if you are allowed to go left and up as well, or INCONCEIVABLE if<br>there simply is no path from s to t.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>.....<br>#..#.<br>#..#.<br>...#.<br>.....

<strong>Output:</strong>
6
</pre>