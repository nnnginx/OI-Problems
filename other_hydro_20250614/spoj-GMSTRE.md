<p>This day is a very special day, especially for all gamers around the world. The clock now is showing at 8 am and the queue in front of the game store is getting crazy. It is like a hundred of people standing in a line waiting for something big. Then what is that ? Yes, of course the people are going to buy the very new game, just released yesterday. It is the first first-person shooting (FPS) game with very incredible price. Brembo, one of the skillfull FPS gamers, of course he doesn't want to miss this. He also buys the game and then plays the game.<br><br>After one hour playing the games, Brembo feels that the game is very difficult, but sometimes is very easy. He doesn't feel good about that, and decided to replay the game from the beginning. However, now he wants to play the game in more balanced ways. He first plays the easy-difficulty levels and then go harder until the he reaches the hardest-difficulty level. Poor Brembo, he finds out that the levels are placed randomly and gets confused on choosing the levels.<br><br>You as his friends, called by Brembo to help him out. There are N levels in the game. Basically, in every level you are given the information about some specific elements. You will notice the bar under the map's levels that contain the information. First, is the number of Health Pack that will be placed in a level. Second, is the number of enemies in a level. And third, is the number of ammo available in a level. A level is said to be easier than another level if it follows these priority, it has more Health Pack, less enemies, and more ammo.<br><br>Now, you are about to analyze the situation based on the description above. Given the information of N levels, find the easiest and the hardest level based on the information. Since you are Brembo's best friend, you don't want to make him disappointed and you will help him.</p>
<h3>Input</h3>
<p>The first line of input is N, the number of levels in the game. (1 &lt;= N &lt;= 100)<br>The next N lines contain three integers separated by space Hi, Ei, Ai, represent the number of Health Pack, enemies, and ammo for i-th level. ( 1 &lt;= Hi,Ei,Ai &lt;= 10000)<br>It is guaranteed that every level has different information.</p>
<h3>Output</h3>
<p>The output contain two lines or one line if there is only one level.<br>First line : "Easiest is level a" (a for the level number)<br>Second Line : "Hardest is level b" (b for the level number)<br>Print them without quotes.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
4
3 2 3
3 4 1
1 4 5
2 2 2

<strong>Output:</strong>
Easiest is level 1
Hardest is level 3
</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
1
2 3 1

<strong>Output:</strong>
Easiest and Hardest is level 1
</pre>