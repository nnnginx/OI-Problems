<p>A wizard is in a labyrinth where there are <em>V</em> rooms and <em>V</em>−1 doors connecting some pairs of rooms in both directions, in such a way that there is always a sequence of doors one can traverse to go from a room to any other room. Additionally, there are <em>C</em> locks and <em>C</em> keys of <em>C</em> different colours (one of each) in some of the doors and rooms of the maze, respectively; each door has at most one lock, and there is at most one key placed in each room. It should be an easy matter for the wizard to bypass the lock system, were it not for the fact that he forgot his spell book, without which his wizardry is utterly useless. The wizard is currently in room <em>X</em>, and he wants to get his spell book, located in room <em>Y</em>, without taking too long. At every step he may go to an adjacent room through one of the doors. Of course, if the door is locked, he needs to be carrying the key of the same colour as the lock (unless, of course, that door has already been unlocked). The wizard can carry only one key at a time and after picking up a key it is not possible for him to drop it somewhere in the maze in order to take it again afterwards. Once a door has been unlocked, the key is thrown away since it is no longer any use.</p>
<p>Given the maze and the positions of the <em>C</em> keys and <em>C</em> locks, determine how to reach <em>Y</em> from <em>X</em>, if possible. Any path whose length does not exceed 4 · (<em>C</em> + 1) · <em>V</em> is acceptable.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each case contains four integers: the number <em>V</em> of rooms in the maze (1 ≤ <em>V</em> ≤ 1&nbsp;500), the number <em>C</em> of locks (0 ≤ <em>C</em> &lt; <em>V</em>), and rooms <em>X</em> and <em>Y</em> numbered 0,1,…,<em>V</em>−1. Then comes a (possibly empty) line with <em>C</em> integers indicating the location of each of the keys, in order of increasing colour. The next <em>V</em> − 1 lines describe the maze: each contains three integers <em>A</em> <em>B</em> <em>L</em>, meaning that there is a door between rooms <em>A</em> and <em>B</em> which can be unlocked with the key of colour <em>L</em>, if 0 ≤ <em>L</em> &lt; <em>C</em>; a value of −1 for <em>L</em> indicates that no lock is needed.</p>
<p>The last line has <em>V</em>, <em>C</em>, <em>X</em>, <em>Y</em> = 0, 0, 0, 0.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>There is one line of output per test case. If there is no solution, output <tt>Impossible</tt>. Otherwise print the full path corresponding to your solution in the format <em>L</em>:&nbsp;<em>V</em><sub>0</sub> … <em>V</em><sub><em>L</em></sub>, where <em>L</em> ≤ 4 (<em>C</em> + 1) <em>V</em> is the length of a path from <em>X</em> to <em>Y</em>, and <em>X</em> = <em>V</em><sub>0</sub>, <em>V</em><sub>1</sub>, …, <em>V</em><sub><em>L</em>−1</sub>, <em>V</em><sub><em>L</em></sub> = <em>Y</em> is the sequence of <em>L</em> + 1 vertices visited in the right order. A single space must precede each vertex in the path; see sample output for clarification.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">1 0 0 0


3 1 0 2
1
0 1 -1
0 2 0

3 2 0 2
1 2
0 1 1
0 2 0

5 3 0 4
2 0 3
0 1 0
0 2 -1
1 3 1
2 4 2

0 0 0 0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">0: 0
3: 0 1 0 2
Impossible
10: 0 2 0 1 0 1 3 1 0 2 4
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Javier Gómez Serrano</em></blockquote>