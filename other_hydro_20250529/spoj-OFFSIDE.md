<p>Hemisphere Network is the largest television network in Tumbolia, a small country located
east of South America (or south of East America). The most popular sport in Tumbolia,
unsurprisingly, is soccer; many games are broadcast every week in Tumbolia.

</p><p></p><p>
Hemisphere Network receives many requests to replay dubious plays; usually, these happen
when a player is deemed to be offside by the referee. An attacking player is <i>offside</i> if he is
nearer to his opponents�� goal line than the second last opponent. A player is not offside if

</p><p></p><p>
</p><ul>
<li> he is level with the second last opponent or
<p></p><p>
</p></li><li> he is level with the last two opponents.
</li></ul>

<p></p><p>
Through the use of computer graphics technology, Hemisphere Network can take an image of
the field and determine the distances of the players to the defending team��s goal line, but they
still need a program that, given these distances, decides whether a player is offside.

</p><h3>Input</h3>
<p>The input file contains several test cases. The first line of each test case contains two integers
A and D separated by a single space indicating, respectively, the number of attacking and
defending players involved in the play (2 &lt;= A,D &lt;= 11). The next line contains A integers B<sub>i</sub>
separated by single spaces, indicating the distances of the attacking players to the goal line
(1 &lt;= B<sub>i</sub> &lt;= 10<sup>4</sup>). The next line contains D integers C<sub>j</sub> separated by single spaces, indicating the
distances of the defending players to the goal line (1 &lt;= C<sub>j</sub> &lt;= 10<sup>4</sup>). The end of input is indicated
by A = D = 0.

</p><h3>Output</h3>
<p>For each test case in the input print a line containing a single character: ��Y�� (uppercase) if
there is an attacking player offside, and ��N�� (uppercase) otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
2 3
500 700
700 500 500
2 2
200 400
200 1000
3 4
530 510 490
480 470 50 310
0 0

<b>Output:</b>
N
Y
N
</pre>