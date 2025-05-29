<p>Mirko has a herd of sheep, surrounded by fences backyard. While he was asleep, wolves have sneaked into the fenced area and attacked the sheep.</p>
<p>Backyard is of a rectangular shape, and consists of fields arranged in rows and columns.</p>
<p>Character '<strong>.</strong>' (fullstop) represents a blank field.</p>
<p>Character '<strong>#</strong>' represents a fance.</p>
<p>Character '<strong>k</strong>' represents a sheep.</p>
<p>Character '<strong>v</strong>' represents a wolf.</p>
<p>&nbsp;</p>
<p>Two fields belong to the same sector if we can move from the field <strong>A</strong> to the field <strong>B</strong> without going over the fence, by making only <strong>horizontal</strong> and <strong>vertical</strong> steps (we cannot move diagonally).</p>
<p>If we can escape from field A from the backyard, that field does not belong to any sector.</p>
<p>Luckily, Mirko taught his sheep Kung-Fu skills, and <strong>they can defend themselves against wolves only if they outnumber the wolves in that sector</strong>. When there are more sheep in the sector than wolves, all wolves die without sheep casualties. Otherwise all sheep perish and wolves are unharmed. If a field doesn't belong in any sector, sheep will flee and wolfs will be left without a prey, so every animal survives.</p>
<p>&nbsp;</p>
<p>Write a program that will determine how many sheep and wolves will survive this bloody night.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Integers N and M, number of rows and columns which represent Mirko's backyard.</p>
<p>In every of the N lines, there are M characters representing the appearence of Mirko's backyard - positions of the fences, wolves and sheep.</p>
<p>&nbsp;</p>
<h3>Constraints</h3>
<p>3 &lt;= N, M &lt;= 250</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>In the first and the only line, print the number of <strong>sheep</strong> and <strong>wolves</strong> that will survive.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>8 8 &nbsp;<br>.######. &nbsp;<br>#..k...# &nbsp;<br>#.####.# &nbsp;<br>#.#v.#.# &nbsp;<br>#.#.k#k# &nbsp;<br>#k.##..# &nbsp;<br>#.v..v.# &nbsp;<br>.######.

<strong>Output:</strong>
3 1
</pre>