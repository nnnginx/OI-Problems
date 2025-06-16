<p>A La Vega Roulette is like a normal Roulette. It is a circular shape with numbers written down on the edge so that they fill up the whole circumference line. It differs from the well-known Roulette in two aspects. First, all numbers have the same color. Second, there is a marker right at the top of the center of the Roulette.</p>
<p>&nbsp;</p>
<p>Natalia and Luis are bored and decided to play "Battle of the Spins" with a La Vega Roulette. On her first turn, a player rotates the La Vega Roulette such that the first number is below the marker. Then, she spins the Roulette and writes down the number that landed on the marker. She also records the position of the Roulette. In subsequent turns, the player must first rotate the Roulette back to the position where it ended in her previous turn, spin, sum the new marked number to her current sum and record again the position.</p>
<p>After both players take a turn then a decision must be made to whether continue playing or announce verdict. Let's say the sum of Player 1 and Player 2 are S1 and S2, respectively. If S1 - S2 &gt; K, Player 1 wins and the game is over. If S2 - S1 &gt; K, then Player 2 wins. However, if S1 - S2 = 0, the game is a draw and ends immediately. If none of the previous conditions apply, the game continues.</p>
<p>You are given the amount of numbers by which the La Vega Roulette spinned after each player's turn. Please output the result of the battle.</p>
<h3>Input</h3>
<p>The first input line contains two space-separated integers N (2 ¡Ü N ¡Ü 10<sup>3</sup>), the size of the list of numbers along the La Vega Roulette's circumference and K (100 ¡Ü K ¡Ü10<sup>5</sup>), the threshold. Then there's a second line with N space-separated 32-bit integers. Each of these integers represent the i<sup>th</sup> number written down on the circumference. &nbsp;Then there are many lines. Each of these lines contain two space-separated integers Spin1 and Spin2 (1 ¡Ü Spin1, Spin2 ¡Ü 10<sup>5</sup>). Each represent the amount of numbers by which the La Vega Roulette rotated in Player 1's and Player 2's turns, respectively. It is guaranteed that there are sufficient lines to reach a verdict.</p>
<h3>Output</h3>
<p>Please output the answer to this problem. If Player 1 wins, write "P1". If Player 2 wins, write "P2". If there's a draw, write "BAD LUCK".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 120</pre>
<pre>6 5 1 80 10 50</pre>
<pre>3 2</pre>
<pre>2 5

<strong>Output:</strong>
P1</pre>
<pre><strong>Note:</strong> In this test case, both players start at the first position. After the first round, Player 1 writes down 80 and Player 2</pre>
<pre>writes down 1. Because S1 - S2 and S2 - S1 are not zero and neither greater than K = 120, the game takes another round. </pre>
<pre>After the second round, Player 1 writes down 50 and Player 2 writes down 5. Now S1 = 80 + 50 = 130 and S2 = 1 + 5 = 6.</pre>
<pre>Because S1 - S2 = 124 &gt; 120, Player 1 wins and the game is over.</pre>