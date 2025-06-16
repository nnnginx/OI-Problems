<p><em>Original problem statements can be found here: <a href="https://contest.pizza/static/tasks/2018/eliminations/pogon.pdf">in Polish</a> and <a href="https://contest.pizza/static/tasks/2018/eliminations/pogon_en.pdf">in English</a></em>.</p>

<p>Archibald the Archeologist was dashing forward as fast as he could, clutching The Idol of Ingenuity tightly. Seizing that artifact almost got him killed<sup>1</sup>, but he still wasn't safe - bunch of South American Indians from Kampa tribe was right on his tail. Fortunately none of them had bows, but they will surely kill him as soon as they catch him. Intricately made figurine was shimmering beautifully in the sun, but at that moment it was only slowing him down - Kampas were faster than him in any case. The situation seemed hopeless...</p>

<p>... but it wasn't. This wasn't a typical jungle - the ground was paved with giant stones, and combined with the surrounding impassable rainforest, it all formed something resembling a corridor. This was surely made by the ancient La-Og-Mhtir civilization, just like the idol. The "corridor" was very long, but very regular - every stone looked like a square, and they were adjoined tightly, one next to the other. Moreover, this corridor  was mentioned in the records Archibald studied for years - it surely was The Way Towards Enlightenment. He already expected to find it on his way to the idol, but maybe the map was upside-down...</p>

<p>... anyway, this is good news. Way Towards Enlightenment isn't just a typical road - it contained a lot of deadly traps. There were levers hidden on some of the stones - every such lever activated a trapdoor hidden below the previous stone. Archibald knows exactly where every lever is.</p>

<p>The situation is as follows - Archibald stands on a plate number <strong>a</strong>. There are <strong>n</strong> Kampas chasing him, and i-th Kampa is on the x<sub>i</sub>-th plate. Every Indian moves onto the next plate every second. Archibald is slower - at the start of every second he can decide to move forward, but he will reach the next plate after two seconds. There are <strong>m</strong> levers, and their positions are denoted by y<sub>i</sub>. If Archibald reaches one of those levers, he can immediately activate the trapdoor - if there is a Kampa on the plate number y<sub>i</sub>-1 at this exact moment, he will fall into a deadly trap. Activating the trap earlier is no good - without the element of surprise, the natives will spot it in advance and run through it safely (probably a bit to the side).</p>

<p>The plan is very simple - neutralize all the Indians without getting caught by them.</p>

<p><sup>1</sup> <small>You can find this story in the problem <a href="http://www.spoj.com/problems/IDO/">"The Idol"</a>, from PIZZA 2017 qualifying round.</small></p>

<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting number of testcases. Then, testcases follow.</p>

<p>The first line of a testcase contains three integers <strong>n</strong>, <strong>m</strong>, <strong>a</strong> ( 1 &lt;= <strong>n</strong> &lt;= <strong>m</strong> &lt;= 1000, 0 &lt;= <strong>a</strong> &lt;= 10<sup>9</sup> ) - number of Indians, number of traps and Archibald's starting plate.</p>

<p>In the next line there are <strong>n</strong> integers <strong>x<sub>i</sub></strong> - plate numbers with Kampas on them at the start. In the last line there are <strong>m</strong> numbers <strong>y<sub>i</sub></strong> - plate numbers with levers.</p>

<p>It is true that:</p>
<p>0 &lt;= x<sub>1</sub> &lt; x<sub>2</sub> &lt; ... &lt; x<sub>n</sub> &lt; <strong>a</strong></p>
<p>0 &lt; y<sub>1</sub> &lt; y<sub>2</sub> &lt; ... &lt; y<sub>m</sub> &lt;= 10<sup>9</sup></p>

<h3>Output</h3>
<p>For every testcase you should find a sequence of moves that will let Archibald trap every Indian. The sequence should start with an integer <strong>r</strong> - number of moves ( 0 &lt;= <strong>r</strong> &lt;= 16<strong>m</strong> ). Then you should give a description of the subsequent <strong>r</strong> moves. Possible moves are as follows:</p>
<ul>
<li>P <em>x</em> - Archibald goes to the right <em>x</em> times. Every move takes him 2 seconds.</li>
<li>S <em>x</em> - Archibald stands still for <em>x</em> seconds.</li>
<li>X - Archibald activates a trapdoor (this happens instantaneously). There has to be a lever on the plate Archibald is standing on. You cannot activate the same trap more than once.</li>
</ul>
<p>In every case <em>x</em> is an integer, and <em>x</em> &gt;= 1.

</p><p>Archibald cannot go to the left, because there is no turning back from The Way of Enlightenment. If at the start of a second Archibald will decide to go to the right, he will still be standing on the same plate at the start of the next second - he will appear on the next plate two seconds after his decision. Indians move at the same time as Archibald - at the start of every second the decide to go right, and at the start of the next second they are at the next plate. At no point should any Kampa stand on the same plate as Archibald. Input is constructed in such a way that a correct sequence always exists.</p>

<h3>Example</h3>
<p>Input:</p>
<pre>1
2 2 8
0 3
12 14</pre>
<p>Output:</p>
<pre>5
P 4
X
P 2
S 1
X</pre>

<h3>Explanation</h3>
<p>Archibald has to run towards the first lever as fast as he can - after 8 seconds from the start he reaches square number 12, and this is the last possible moment - Kampa closest to him reached plate number 11 already. After he reaches the second trap he has to wait for a second, so the Indian is right above the trapdoor.</p>