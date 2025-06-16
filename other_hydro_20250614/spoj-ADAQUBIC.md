<p>Ada the Ladybug was playing <a href="https://en.wikipedia.org/wiki/3D_tic-tac-toe">3D Tic-Tac-Toe</a> against her good friend Velvet Mite Vinit. They were playing on 3x3x3 field. Sadly, Vinit had to go home earlier so the game was left unfinished. Ada wants to know who would win the match (if they both played optimaly). You also know that Ada started.</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>1 ¡Ü T ¡Ü 1000</strong>, number of test-cases.</p>
<p>Each test-case will contain 9 lines with three character each, representing the field (<strong>'.'</strong> for empty place, <strong>'x'</strong> for move of Ada and <strong>'o'</strong> for move of Vinit). You are assured that the game is unfinished and valid.</p>
<p>First three lines represent the top field, the next three lines represent middle field and the last three lines represent the bottom field.</p>
<p>There will be a blank line before each test-case.</p>
<h3>Output</h3>
<p>For each test-case, print the name of winner (<strong>Ada</strong> or <strong>Vinit</strong>);</p>
<h3>Example Input</h3>
<pre>7

..o
o.x
xox
x.x
...
x.o
...
o.o
.x.

.x.
...
..o
o.x
x..
..o
..x
...
...

o..
...
o.x
.x.
...
.x.
o.o
.xx
oox

..x
..x
.o.
..x
..x
xo.
o..
..o
...

...
..x
..x
.o.
..x
o..
...
...
x.o

...
..x
..o
...
...
xo.
ox.
...
.ox

o..
x..
...
oxx
..o
.ox
..o
.x.
.x.
</pre>
<h3>Example Output</h3>
<pre>Vinit
Vinit
Ada
Vinit
Ada
Vinit
Vinit
</pre>
<h3>Example Input 2</h3>
<pre>1

xox
x.o
oox
o.o
x.x
xxo
x.o
oxo
ox.
</pre>
<h3>Example Output 2</h3>
<pre>Ada
</pre>