<p> Ada the Ladybug has decided to move to other city. She was deciding where
to live - she wanted the city which would be the biggest PLUS to live in. You
will be given a map with <b>N¡ÁN</b> cities. Size of PLUS is the number of cities in each of four direction (+ the city itself).</p>


<h3>Input</h3>
The first line contains <b>T</b>, the number of test-cases.

<p>The first line of each test-case will contain <b>0 &lt; N ¡Ü 2000 </b>, the
size of map.

</p><p><b>N</b> lines will follow, each containing <b> N </b> characters. Characters
will be either '#' (indicating a city) or '.' (indicating free space).

</p><h3>Output</h3>
For each test-case, print exactly one number - the size of biggest '+' (PLUS).
<h3>Example Input</h3>
<pre>4
5
..#..
..#.#
#####
..#.#
..#..
3
..#
#.#
#.#
4
##.#
####
##.#
#..#
4
####
####
####
####
</pre>
<h3>Example Output</h3>
<pre>3
1
2
2
</pre>
<h3>Explanation of test-cases</h3>
<b>1st test-case</b>
<pre>..<font color="red">#</font>..
..<font color="red">#</font>.#
<font color="red">#####</font>
..<font color="red">#</font>.#
..<font color="red">#</font>..
</pre>
<p><b>2nd test-case</b>
</p><pre>..#
#.<font color="red">#</font>
#.#
</pre>
<p><b>3rd test-case</b>
</p><pre>#<font color="red">#</font>.#
<font color="red">###</font>#
#<font color="red">#</font>.#
#..#
</pre>
<p><b>4th test-case</b>
</p><pre>#<font color="red">#</font>##
<font color="red">###</font>#
#<font color="red">#</font>##
####
</pre>