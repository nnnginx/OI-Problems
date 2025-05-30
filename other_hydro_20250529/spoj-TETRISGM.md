<p>Alice and Bob are playing game with each other. They play the game on a 2D board. Alice has many vertical 1*2 tiles while Bob has many horizontal 2*1 tiles. They take turn to place their own tiles on the board. Considering about that the tiles cannot overlap each other, the player cannot do the placement any more loses. Since this is such a complex game that they could not find optimal method to play that, Alice decide to simplify this game by replace the large 2D board by some small ones. Alice set up a lot of Tetris tiles instead of the original 2D board. In the other words, the player can only place their own vertical or horizontal tiles on the Tetris-like board. Each player can choose one possible place on any Tetris tiles to place its own tiles. In fact, there are following 15 types of Tetris playground.</p>
<p><img src="../../../content/john_jones:tetrisgm.jpg" alt=""></p>
<p>The playground cannot be transformed in any ways, including reflection and rotation.</p>
<p>Given the number of each type of tiles, you are asked to determine who will win the game if Alice plays first and both players are playing optimal.</p>
<h3>Input</h3>
<p>There are multiple test cases; the first line of input contains a single integer denoting the number of test cases.</p>
<p>For each test case, there are only one line contains 15 integers denoting the number of Tetris tiles of the above 15 types. All the numbers are no greater than 100.</p>
<h3>Output</h3>
<p>For each test cases, output <strong>Alice</strong> if Alice will win the game and both player plays optimally, <strong>Bob</strong> otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 4 0 0 0 0 0 0 0 0 0 0 0 0 0
5 5 0 0 0 0 0 0 0 0 0 0 0 0 0
100 100 0 0 0 0 0 0 0 0 0 2 1 0 0

<strong>Output:</strong>
Case #1: Alice
Case #2: Bob
Case #3: Alice
</pre>