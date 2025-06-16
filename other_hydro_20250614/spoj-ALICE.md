<p>Alice and Bob are very smart guys and they like to play all kinds of games in their spare time. The  most amazing thing is that they always find the best strategy, and that's why they feel bored again and again. They just invented a new game, as they usually did.</p>

<p>The rule of the new game is quite simple. At the beginning of the game, they write down <b>N</b>
random positive integers, then they take turns (Alice first) to either:</p>

<ol>
<li>Decrease a number by one.</li>
<li>Erase any two numbers and write down their sum.</li>
</ol> 

<p>Whenever a number is decreased to 0, it will be erased automatically. The game ends when all numbers are finally erased, and the one who cannot play in his(her) turn loses the game. </p>

<p>Here's the problem: Who will win the game if both use the best strategy? Find it out quickly, before they get bored of the game again!</p>



<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 4000), indicating the number of test cases. 
Each test case contains several lines.
The first line contains an integer <b>N</b> (1 ¡Ü <b>N</b> ¡Ü 50).
The next line contains <b>N</b> positive integers <b>A<sub>1</sub></b>... <b>A<sub>N</sub></b> (1 ¡Ü <b>A<sub>i</sub></b> ¡Ü 1000), represents the numbers they write down at the beginning of the game.
</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is either <tt>"Alice"</tt> or <tt>"Bob"</tt>.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
3
1 1 2
2
3 4
3
2 3 5

<b>Output:</b>
Case #1: Alice
Case #2: Bob
Case #3: Bob
</pre>