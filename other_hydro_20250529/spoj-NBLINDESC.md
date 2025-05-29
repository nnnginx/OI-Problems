Illidan Stormage, the blind Warcraft hero is thrown in a maze for punishment. Being a blind hero, he cannot see anything but he can sense which direction is North, East, South and West.
<br><br>

Assume that the maze is laid out on a  <strong>N x M</strong> grid, and each grid location is either blocked or free. Illidan starts from a free location at time 0, and his goal is to escape from the maze. He has four possible moves - move to North, East, South or West. Making a move to an adjacent cell takes <strong>exactly 1 unit</strong> of time. If Illidan attempts to move out of the grid or attempts to move into an obstacle, he will stay in his current location but it will still cost him 1 unit of time. There is exactly one exit in the maze, located in one of the free cells. Illidan escapes <strong>immediately</strong> whenever he reaches the exit.
<br><br>

Keep in mind that Illidan is blind, so he may get confused while making a move. To avoid all this chaos, he decided to follow a rather simple strategy. Before he starts his journey to escape the maze, he selects four real numbers: <strong>P<sub>N</sub></strong>, <strong>P<sub>E</sub></strong>, <strong>P<sub>S</sub></strong> and <strong>P<sub>W</sub></strong> denoting the probability to move North, East, South and West respectively. No matter where he is, he will always attempt to move North with probability <strong>P<sub>N</sub></strong>, East with probability <strong>P<sub>E</sub></strong>, South with probability <strong>P<sub>S</sub></strong>, and West with probability <strong>P<sub>W</sub></strong>. At any moment, Illidan must attempt to make a move in one of these four directions. In other words, this means that  <strong>P<sub>N</sub> + P<sub>E</sub> + P<sub>S</sub> + P<sub>W</sub> = 1 must be equal to 1</strong>.
<br><br>

Illidan does not want to be stuck in the maze for too long. He has information about the maze so he knows his starting position, the location of the exit cell and all the free cells and obstacles initially. Before he attempts to escape, he would like to set the values <strong>P<sub>N</sub></strong>, <strong>P<sub>E</sub></strong>, <strong>P<sub>S</sub></strong> and <strong>P<sub>W</sub></strong> such that the <strong>expected time for him to escape the maze is minimized</strong>.
<br><br>

Given the description of the maze, Illidan¡¯s starting position and the location of the exit cell, calculate the minimum expected time for Illidan to escape. You can safely assume that Ilidan¡¯s starting cell and the exit cell will <strong>always be connected</strong>, that is, it will be possible to reach the exit cell via some sequence of moves.
<br><br>

<h3>Input</h3>
The first line of the input contains an integer <strong>T</strong>, denoting the number of test cases. Then the description of <strong>T</strong> test cases follow. The first line of every test case will start with a blank line.
The second line contains two space separated integers, <strong>N</strong> and <strong>M</strong> denoting the number of rows and the number of columns of the grid. Each of the next <strong>N</strong> lines will contain exactly <strong>M</strong> characters on each line describing the grid. The grid will only consist of the characters <strong>.</strong> <strong>@</strong> <strong>#</strong> and <strong>*</strong>. 
<br><br>
<strong>.</strong> indicates a free cell.
<br><br>
<strong>@</strong> indicates Illidan¡¯s starting position which is also a free cell and will occur exactly once.
<br><br>
<strong>#</strong> denotes an obstacle.
<br><br>
<strong>*</strong> denotes the location of the exit cell, is of course a free cell and will occur exactly once.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 32</li></strong>
<strong><li>1 ¡Ü N, M ¡Ü 8</li></strong>

<h3>Output</h3>
For each test case, print the expected time for Illidan to escape the maze if he chooses the probabilities optimally in a single line. <strong>Absolute</strong> error less than <strong>10<sup>-6</sup></strong> will be ignored.

<h3>Sample Input</h3>
<pre>2

1 2
@*

3 3
@..
#.#
..*
</pre>

<h3>Sample Output</h3>
<pre>1.0000000000000
16.360252929211
</pre>

<h3>Credits</h3>
Problem name and story inspired by <a href="http://www.lightoj.com/volume_showproblem.php?problem=1426&amp;language=english&amp;type=pdf">LightOJ 1426 - Blind Escape</a>
<br><br>
Or if you prefer a blinder (easier) version <a href="https://www.spoj.com/problems/BLINDESC/">SPOJ BLINDESC - Blind Escape II</a>
<br><br>