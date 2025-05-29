<p align="justify">
You recently watched a video clip in which a singer danced on a grid of colourful tiles enlightened from below. Each step on a tile flipped the tile's state, i.e. light on or off. In addition to that, all the neighbouring tiles flipped their states, too.
<br><br>
In this task, you are supposed to come up with a short program that decides if it is possible for the singer to switch on the lights of all the tiles, provided that he dances on the appropriate tiles.
<br><br>
The dance floor has rectangular shape. At the beginning, some of the tiles are already alight. Your program may temporarily switch off some tiles, if it deems that necessary to reach its goal. Stepping on a tile toggles its own state as well as the states of the four neighbouring tiles directly above, below, to the left and to the right. Of course, in the case of a peripheral tile, there will be only three or two neighbouring tiles.
<br><br>
Here comes an example:
<br>
<img src="/content/ahven:example.gif">
<br>
If the dancer steps on the tile indicated by the brown shoe, all the tiles within the white area change their states. The resulting dance floor is depicted on the right.
<br><br>
You may assume that the singer is fit enough to jump from any tile to any other tile, even if the destination tile lies on the opposite side of the dance floor.
</p>
<h3>Input</h3>
<p align="justify">
There are several test cases.
The first line of each case contains two integer numbers <em>x</em> and <em>y</em>,
  indicating the width and the height of the dance floor grid. The numbers are
  separated by a single space and satisfy 3 ¡Ü <em>x</em>,<em>y</em> ¡Ü
  15.
<br><br>
The following <em>y</em> lines containing <em>x</em>characters each describe
  the initial on/off states of the tiles. A zero means "the tile is switched
  off", a one digit means "the tile is alight".
<br><br>Input ends with 0 0.
</p>
<h3>Output</h3>
<p align="justify">
For each test case your program should output the number of steps needed to switch all the lights on, followed by exactly that many lines with two space-separated numbers <em>i</em> and <em>j</em>. Each individual line commands the singer to
  step on the <em>i</em>-th tile of the <em>j</em>-th row. Starting with the situation
  of the input file and executing all the commands in the output file, all the
  tiles must be switched on.
<br><br>
If more than one solution exist, your program should output an arbitrary one
  of them. If, on the other hand, no solution exists, your program should write the number "-1".
</p>
<h3>Example</h3>
<pre><h4>Sample input</h4>
4 3
0111
1010
1000

0 0

<h4>Sample output</h4>
3
1 2
1 3
4 3
</pre>