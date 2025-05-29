<p>Today, Waca will play runner game. In this game, the player will be placed in a square-shaped arena where they will run to checkpoints of the arena.</p>
<p>Arena of the game is a square with a side length of N. The player will be placed in a coordinate (X,Y) inside the arena. The following are the rules of the game :</p>
<ul>
<li>Player will be initially at coordinate (X,Y), where coordinate (0,0) is the bottom left corner of the arena</li>
<li>Then, player should run to the side of the arena to get the checkpoints</li>
<li>Checkpoints are located in each side of the arena (top, left, bottom, right) and player should take all the checkpoints (i.e. they have to visit all sides), then go back to the initial position of the player (X,Y)</li>
<li>If the player reach the corner of the arena, he can take 2 checkpoints. For example, if a player reach coordinate (0,0), he is considered to get the left and bottom checkpoints</li>
</ul>
<p>Now, Waca is curious, what is the minimum distance to get all the checkpoints and go back to his initial position? The image below is one of the possible moves for the runner game. (The red circle is Waca's initial position (X,Y) )</p>
<p><img src="file://mDLa6YOX.png" alt="Sample run" width="296" height="288"></p>
<h3>Input</h3>
<p>The input will contain 3 integers, X, Y, and N.</p>
<h3>Output</h3>
<p>Print the minimum distance Waca need to finish the game. Your answer is considered to be correct if the difference is no more than 10<sup>-6</sup></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 4 10

<strong>Output:</strong>
28.284271</pre>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>1 ¡Ü N ¡Ü 10<sup>6</sup></li>
<li>0 ¡Ü X,Y ¡Ü N</li>
</ul>
</div>