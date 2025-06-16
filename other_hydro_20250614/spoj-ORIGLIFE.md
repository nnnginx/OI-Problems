<p>Conway's <i>Game of Life</i> is not really a game, but a <i>cellular automaton</i> -- a set of rules describing interactions among adjacent cells on a grid. In our game, we have an <i>n</i> by <i>m</i> rectangular grid of cells identified by integer coordinates (<i>x, y</i>). The game progresses through a series of steps; at each step a new <i>generation</i> is computed from the current <i>generation</i>. The game begins with the <i>first generation</i>. In any given generation, which we shall call the current generation, each cell is either <i>live</i> or <i>dead</i>. In the next generation, each cell's status may change, depending on the status of its immediate neighbours in the current generation. Two distinct cells (<i>x<sub>1</sub>, y<sub>1</sub></i>) and (<i>x<sub>2</sub>, y<sub>2</sub></i>) are immediate neighbours if they are horizontally, vertically, or diagonally adjacent; that is, if |<i>x<sub>1</sub> - x<sub>2</sub></i> ¡Ü 1| and |<i>y<sub>1</sub> - y<sub>2</sub></i> ¡Ü 1|. Each cell that is not on the border of the grid has eight immediate neighbours. There are three integer parameters (<i>a, b, c</i>) which affect the game. The rules of the game are:
</p><ul>
<li>If a live cell has fewer than <i>a</i> live neighbours in the current generation it dies of loneliness. That is, it is dead in the next generation.</li>
<li>If a live cell has more than <i>b</i> live neighbours in the current generation it dies of overcrowding. That is, it is dead in the next generation.</li>
<li>If a dead cell has more than <i>c</i> live neighbours in the current generation it is born. That is, it is live in the next generation.</li> 
<li>Otherwise, a cell's status is unchanged from the current generation to the next.</li>
</ul>
<p>This process continues indefinitely. Eventually, a generation may be repeated in which case life goes on forever. Or all the cells may die. Similarly, if we explore previous generations that may have led to the current one, we may find one that is necessarily a first generation; that is, it could not have been created from a previous generation by following the rules. Such a generation is known as a Garden of Eden. Given the game parameters and the current generation, you are to determine whether or not the game might have started with a Garden of Eden. If so, output the number of steps necessary to reach the current generation from the Garden of Eden. If there are several possible answers, find the smallest. If there is none, output -1.

</p><h3>Input</h3> <p>Input begins with a single integer, the number of test cases. For each test case, there are <i>m</i>+1 lines of input in total. The first line contains the game parameters, which are five integers <i>m,n,a,b,c</i> each separated by one space. The constraints are 1¡Ü<i>m</i>¡Ü4, 1¡Ü<i>n</i>¡Ü5, 1¡Ü<i>a</i>&lt;<i>b</i>¡Ü8, 1¡Ü<i>c</i>¡Ü8. The next <i>m</i> lines each contain a string of <i>n</i> characters representing a row of the current generation. In the string, an asterisk ("*") indicates live while a period (".") indicates dead.
There are no blank lines between test cases.

</p><h3>Output</h3>
<p>Output is one integer per test case denoting the minimum number of steps required to reach the input from a Garden of Eden. If there is no Garden of Eden, output -1.

</p><h3>Example</h3>
<pre><b>Input:</b>
1
4 5 2 3 2
.****
.****
.****
.****

<b>Output:</b>
2

<b>Output Explanation:</b>
</pre>
<p>Assume the sample input is the "current" generation. A possible previous generation is
</p><pre>**.**
..*.*
....*
*****
</pre>
<p>The above generation can be derived from the following previous generation
</p><pre>.****
**.*.
*****
*..*.
</pre> 
<p>
This generation cannot be derived from any other generation. Furthermore, there is no shorter
series of generations that has these properties.

</p>