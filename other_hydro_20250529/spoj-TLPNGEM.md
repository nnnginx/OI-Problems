<p>Duck is playing "Teleporters and Gems". On a 1 x <strong>N</strong> map, there may be multiple teleporters (or no) and at least one gem. At the beginning, Duck is standing at the most left position. He has to collect all the gems with the help of teleporters. Below are the rules:</p>
<p>1. Moving 1 unit is counted as 1 move</p>
<p>2. When Duck reaches a teleporter, he can instantly reach any of the next 3 teleporters (eg. 1 to 2, 3 or 4 teleporter, but not 1 to 5, 6, 7 teleporter, and previous not allowed) by 3 moves; Or he can ignore that teleporter and keep moving to next cell which is counted as 1 move</p>
<p>&nbsp; &nbsp; Let '@' = Teleporter, '.' = empty cell, there are 4 teleporters: @.@..@@, if Duck is at position 0 (the 1-st teleporter), then he can instantly reach 2-nd, 3-rd or 4-th teleporter by 3 moves. But ignoring the 1-st teleporter makes him reach 2-nd teleporter by 2 moves.</p>
<p>3. Duck has to collect all gems</p>
<p>4. Once he collects the last gem, the game ends and no more move needed</p>
<p>Can you help him find out the minimum number of moves in order to collect all gems?</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü T ¡Ü 50)</p>
<p>For each test case, there is a string <strong>S</strong> consisting of '.' (¡Ý 0), '@' (¡Ý 0) and '*' (¡Ý 1), representing empty cell, teleporter and gem. (1 ¡Ü |S| ¡Ü 10<sup>4</sup>)</p>
<h3>Output</h3>
<p>Print one integer x where x is the minimum number of moves in order to collect all gems starting from the most left cell.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
.@@...@.@...@@..*@.@.*...@..
....@...@@.**.@....@@@*@.
.*....*@@@@*..@@*..@

<strong>Output:</strong>
14
16
16
</pre>
<h3>Explanation</h3>
<p>Bracket means cells that Duck will pass through and minimum number of moves to that cell<br> Case 1: (.@@)...@.@...(@@..*@.@.*)...@.. = 0 1 2 -&gt; 5 6 7 8 9 10 11 12 13 14<br> Case 2: (....@)...@(@.**.@)....@@(@*)@. = 0 1 2 3 4 -&gt; 7 8 9 10 11 12 -&gt; 15 16<br> Case 3: (.*....*@)@@(@*..@@*)..@ = 0 1 2 3 4 5 6 7 -&gt; 10 11 12 13 14 15 16</p>