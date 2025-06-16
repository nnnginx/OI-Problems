<p><em>Original problem statement (in Polish) can be found <a href="https://pizza.natodia.net/static/tasks/2016/eliminations/laser.pdf">here</a>. (It contains some more story that was removed from this version, because certain pun does not make any sense in English).</em></p>
<p>There is a grid with <strong>n</strong> rows and <strong>m</strong> columns, consisting of 1x1 squares. There is exactly one square with a laser and one (different) square with a sensor. The laser emits a beam of concentrated light from the middle of its square, in one of the four directions (north, south, east or west). Some squares are blocked, so they don't let the light through. (In that sense, square with a laser is also considered blocked).</p>
<p>We have a number of two-sided mirrors. We can place them on the middle of a square, in one of the two configurations (45 degrees). Mirrors placed in such a way reflect the light, making a right angle (90 degrees).</p>
<p>Your task is to guide the light to the sensor, using the minimum number of mirrors.</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, testcases follow.</p>
<p>The description of a single testcase begins with two integers <strong>n</strong>, <strong>m</strong> (1 &lt;= <strong>n</strong>, <strong>m</strong> &lt;= 200) - number of rows and columns, respectively. Then, <strong>n</strong> lines follow, each containing <strong>m</strong> characters. <strong>j</strong>-th character in <strong>i</strong>-th line denotes a square in <strong>i</strong>-th row nad <strong>j</strong>-th column. "." (a dot) denotes free square, "#" denotes blocked square. There is exactly one laser on the grid, represented by one of these four characters: "&lt;", "&gt;", "v" or "^" (it depends on the direction of the laser). There is also exactly one sensor, represented by "C". No other characters can appear in a line.</p>
<h3>Output</h3>
<p>For every testcase you should print <strong>n</strong> lines with <strong>m</strong> characters, denoting the grid from the input, but with mirrors placed on some of the fields. Mirrors are represented by "\" and "/" characters. Arrangement of mirrors should make the light reach the sensor, while using minimum possible number of mirrors. You can't place mirrors on blocked fields, as well as on field with the laser and on field with the sensor. There is always a way for the light to reach the sensor.</p>
<h3>Example</h3>
<p>Input:</p>
<pre>2
3 4
&gt;...
###.
C...
5 5
v#...
.#.#.
.#.#.
.#.#.
...#C</pre>
<p>Output:</p>
<pre>&gt;..\
###.
C../

v#/.\
.#.#.
.#.#.
.#.#.
\./#C</pre>