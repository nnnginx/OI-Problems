<p>After duelling in quake (a multiplayer game), Airborne and Pagfloyd decide do test themselves out in another game called Hubulullu.  The rules of the game are as follows:</p>

<p><b>N</b> wooden pieces (marked with numbers 1 to N) are placed in a transparent bottle.  On his turn the first player takes out some piece (numbered x) and all the pieces numbered by divisors of x that are present in the transparent bottle.  The second player picks another number and removes it and its divisors as well.  Play continues in an alternating fashion until all pieces have been removed from the bottle.  The player who removes the last piece from the bottle wins the game.</p>

<p>Both players play optimally.  Given <b>N</b> (the number of wooden pieces in the transparent bottle initially) and the name of the player who starts the game, determine the winner.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>Each test case consists of a single line containing two integers separated by a single space.  The first integer is <b>N</b> (1 &lt;= <b>N</b> &lt;= 2000000000), indicating the number of pieces, and the second integer indicates the player who starts - "0" means Airborne starts the game and "1" means Pagfloyd starts the game (quotes for clarity).

</p><h3>Output</h3>
<p>For each test case output one line containing either "Airborne wins." or "Pagfloyd wins."</p>

<p>For each N, it's possible to determine a winner if both players play optimally.</p>


<h3>Example</h3>

<pre><b>Input:</b>
1
1 0

<b>Output:</b>
Airborne wins.
</pre>