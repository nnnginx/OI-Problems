Illidan Stormage, the blind Warcraft hero is thrown in a maze for punishment. Being a blind hero, he cannot see anything but he can sense which direction is North, East, South and West.
<br><br>

Assume that the maze is laid out on a grid, and each grid location is either blocked or free or contains a demon. He has four possible moves: North, East, South, and West. Illidan starts from a free location at time <strong>t=0</strong>, and his goal is to kill all the demons within time <strong>T</strong>. Illidan kills a demon immediately (takes <strong>0 unit</strong> of time) whenever he lands on a grid location containing a demon, however making a move to an adjacent cell takes exactly <strong>1 unit</strong> of time. If Illidan attempts to move out of the grid or attempts to move to an obstacle, he will stay in his current location but it will still cost him <strong>1 unit</strong> of time. When Illidan kills the last demon, he is <strong>immediately</strong> freed from the maze but if he fails to kill all the demons within time <strong>T</strong>, he will be trapped in the maze for eternity.
<br><br>

Keep in mind that Illidan is blind, so he may get confused while making a move. To avoid all this chaos, he decides to follow a rather simple strategy. Before he starts his journey to hunt and kill all the demons, he selects four real numbers: <strong>P<sub>N</sub></strong>, <strong>P<sub>E</sub></strong>, <strong>P<sub>S</sub></strong> and <strong>P<sub>W</sub></strong> denoting the probability to move North, East, South and West respectively. No matter where he is, he will always attempt to move North with probability <strong>P<sub>N</sub></strong>, East with probability <strong>P<sub>E</sub></strong>, South with probability <strong>P<sub>S</sub></strong>, and West with probability <strong>P<sub>W</sub></strong>.
<br><br>

Given the description of the maze, the location of all the demons, Illidan¡¯s starting position and the probabilities of each move, calculate the probability that Illidan will be able to kill all the demons before the time runs out.
<br><br>

Assume the grid will be of dimensions <strong>N x M</strong> and will contain <strong>K</strong> demons.
<br><br>

<h3>Input</h3>
The first line of the input contains an integer <strong>Q</strong>, denoting the number of test cases. Then the description of <strong>Q</strong> test cases follow. The first line of every test case will start with a blank line.
<br><br>

The second line contains three space separated integers, <strong>N</strong>, <strong>M</strong> and <strong>T</strong>, denoting the number of rows, the number of columns of the grid and the time by which Illidan needs to kill all the demons respectively. The third line contains four space separated real numbers <strong>P<sub>N</sub></strong>, <strong>P<sub>E</sub></strong>, <strong>P<sub>S</sub></strong> and <strong>P<sub>W</sub></strong> in that order. All these numbers will contain at most <strong>2 digits</strong> after the decimal point.
<br><br>

Each of the next <strong>N</strong> lines will contain exactly <strong>M</strong> characters on each line describing the grid. The grid will only consist of the characters <strong>.</strong> <strong>@</strong> <strong>#</strong> and <strong>*</strong>. 
<br><br>
<strong>.</strong> indicates a free cell.
<br><br>
<strong>@</strong> indicates Illidan¡¯s starting position which is also a free cell and will occur exactly once.
<br><br>
<strong>#</strong> denotes an obstacle.
<br><br>
<strong>*</strong> denotes the location of a demon, there can be at most one demon in a cell.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü Q ¡Ü 5</li></strong>
<strong><li>1 ¡Ü N, M ¡Ü 8</li></strong>
<strong><li>1 ¡Ü T ¡Ü 16777216</li></strong>
<strong><li>1 ¡Ü K ¡Ü 3</li></strong>
<strong><li> P<sub>N</sub> + P<sub>E</sub> + P<sub>S</sub> + P<sub>W</sub> = 1 </li></strong>

<h3>Output</h3>
For each test case, print the probability of Illidan escaping the maze in a single line. Error less than <strong>10<sup>-6</sup></strong> will be ignored.

<h3>Sample Input</h3>

<pre>3

1 2 3
0 0.5 0 0.5
@*

1 8 64
0 0.5 0 0.5
@......*

8 8 10000000
0.05 0.25 0.45 0.25
##....#.
.##.....
.*#.##..
.##..*#.
...###..
.#.#....
.#.#.#..
@#.*.#..
</pre>

<h3>Sample Output</h3>
<pre>0.875000000000
0.693211582717
0.157323987423
</pre>

<h3>Credits</h3>
Problem name and story inspired by <a href="http://www.lightoj.com/volume_showproblem.php?problem=1426&amp;language=english&amp;type=pdf">LightOJ 1426 - Blind Escape</a>
<br><br>
Or if you prefer a not so blind version <a href="https://www.spoj.com/problems/NBLINDESC/">SPOJ NBLINDESC- Not So Blind Escape</a>
<br><br>