<p>Duck is playing a game named "Supraiden", which is another version of a famous shooting game named "Raiden". On a <strong>D</strong> ¡Á 10<sup>9</sup> map, initially Duck is at the left top coordinates (1, 1), and there are <strong>N</strong> enemies at the bottom of the map but with different horizontial position <strong>L</strong><sub>i</sub>. That is, the first enemy is at (D, L<sub>1</sub>), the second one is at (D, L<sub>2</sub>), and so on. The i-th enemy has <strong>M</strong><sub>i</sub> bullets, and he will shoot the j-th bullet at time&nbsp;<strong>S</strong><sub>ij</sub>.</p>
<p>All enemies are fixed, so they cannot move; and Duck can choose to stay at the same position, or move one unit on map horizontally&nbsp;per unit of time. For example, moving from (1, 1) to (1, 5) takes 4 units of time. But Duck can only move to a cell where currently no bullets at there.<br>Assume Duck will move to right at next unit of time, the following are two examples will cause valid move, followed by two invalid move examples:</p>
<pre>(D = Duck, E = enemy, ^ = bullet from enemy)
    Valid              Invalid (Duck will get hit)
..D..   ..D^.       ..D..   ..D^.
.....   .^^..       ...^.   ...^.
...^.   .....       ..^..   ...^.
.EEE.   .EEE.       .EEE.   .EEE.
</pre>
<p>Bullet speed is one unit on map per unit of time. Shooting takes 0 unit of time, but Duck and enemies can only shoot one bullet per unit of time and shoot vertically. For example, moving from (1, 1) to (1, 5) and shoot immediately only takes 4 units of time. When two bullets collide with each other, both disappear. Collision only occurs when one side shoots before the bullet from another side reaches his current position.<br>Assume Duck will shoot at next unit of time, the following are&nbsp;two examples will cause valid collision, followed by two invalid collision examples:</p>
<pre>(D = Duck, E = enemy, v = bullet from Duck, ^ = bullet from enemy)
    Valid              Invalid (Duck will get hit)
..D..   ..D..       ..D..   ..D..
..v..   .....       ..^..   ..^..
..^..   ..^..       .....   ..^..
..E..   ..E..       ..E..   ..E..</pre>
<p>Duck has infinite amount of bullets, starting at time 0, your task is find the minimum time to kill all enemies without getting hit.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>.  (1 ¡Ü T ¡Ü 20)</p>
<p>For each test case, it starts with two integers&nbsp;<strong>D</strong>, <strong>N</strong>. (3 ¡Ü D ¡Ü 10<sup>9</sup>, 1 ¡Ü N ¡Ü 8)</p>
<p>Following N lines, each starts with <strong>L<sub>i</sub></strong>, <strong>M<sub>i</sub></strong>, followed by M<sub>i</sub>&nbsp;distinct integers <strong>S<sub>ij</sub></strong>. (1 ¡Ü L<sub>i</sub> ¡Ü 10<sup>9</sup>, 1 ¡Ü M<sub>i</sub>, ¡Ü 1000, 1 ¡Ü S<sub>ij</sub> ¡Ü 10<sup>9</sup>)</p>
<p>*L<sub>i</sub> and S<sub>ij</sub> are already sorted in ascending order.</p>
<h3>Output</h3>
<p>Output the minimum time to kill all enemies.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
100 1
1 1 100
5 3
12 9 0 1 4 5 6 7 8 9 19
14 2 12 88
20 5 23 27 29 35 100
6 2
6 7 1 2 3 4 5 6 7
8 1 0

<strong>Output:</strong>
99
29
18
</pre>
<h3>Explanation</h3>
<p>In case 1, Duck can shoot one bullet at time 0.</p>
<p>In case 2, Duck reaches (1, 12) at time 14, and shoots. Then he moves and reaches (1, 14) at time 17 and shoots. Lastly he reaches (1, 20) at 23 and shoots three bullets. The first two bullets collided with the first two bullets shooted by enemy 3, and the last bullet hits the enemy at time 29.</p>
<p>In case 3, Duck reaches (1, 6) but doesn't shoot, then moves to (1, 8) immediately and shoots one bullet. After that, he goes back and reaches (1, 6) at time 13 and shoots. The bullet hits enemy 1 at time 18.</p>