<p>Ada the Ladybug loves Crosswords, Sudoku's and all other similar games. She has found an interesting game in the latest issue of Magazine Bug.</p>
<p>The game is simple - you will be given a square full of numbers. Each number must be part of exactly one path. Path must begin at number <strong>1</strong> and can only continue to neighboring number (left,right,up,down), which is larger by 1.</p>
<p>Ada's friend is working as a director of Magazine Bug. He wants to surprise her and add few more games to following issues of the magazine. Anyway, he wants you to check, whether the games are valid (i.e. if all the numbers can be part of a path).</p>
<h3>Input</h3>
<p>The first line will contain <strong>T</strong>, the number of test-cases.</p>
<p>Then <strong>T</strong> test-cases follow, each beginning with an integer <strong> 1     ¡Ü N ¡Ü 100</strong>, the size of the game board.</p>
<p>Afterward, <strong>N</strong> lines follow with <strong>N</strong> integers <strong>1 ¡Ü     A<sub>ij</sub> &lt; 10</strong></p>
<h3>Output</h3>
<p>For each test-case print either "<strong>YES</strong>" if board is valid or "<strong>NO</strong>" if it isn't.</p>
<h3>Example Input</h3>
<pre>4
4
1 2 3 4
4 3 2 1
1 2 2 1
1 1 1 2
3
1 2 3
4 5 6
1 2 1
2
1 2
4 3
2
1 2
2 2
</pre>
<h3>Example Output</h3>
<pre>YES
NO
YES
NO
</pre>