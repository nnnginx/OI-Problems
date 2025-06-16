<p>After the end of all the shooting competitions in XXIX Olympic Games in Beijing, Matthew Emmons will be known to more and more people because of his last - which is also his worst - shooting in the 50m Rifle 3*40 Men competitions. Four years before in Athens, he shot a wrong target and lost the gold metal which is almost at hands in the 50m Rifle 3*40 Men competition.</p>
<p><b>The following is Blue Mary's imagination :P</b></p>
<p>Emmons decides to practise shooting more assiduously. Because he is an excellent shooter, only 1 year later, he can even shoot precisely without collimation! To him, getting the gold metal of 50m Rifle 3*40 Men in XXX Olympic Games doesn't have any difficulty now.</p>
<p>His wife - Katerina Emmons, also a well-known excellent shooter - make a game to keep his interests with shot. The player has <i>n</i> (1&lt;= <i>n</i> &lt;=2000) bullets, each one has a value (a integer whose absolute value is less than 10000). There are <i>m</i> (1&lt;= <i>m</i> &lt;= <i>n</i>) targets, each with a point counter next to it. In the beginning of the game, all the counter are set to integer 1.</p>
<p>During the game, the player must choose a bullet and shoot any target. He must use all the bullet, each with at least(of course, at most) 1 time. And each target must be shot at least one time.</p>
<p>If the player shoot a target with a bullet valued <b>X</b>, the counter of the target will multiplied by <b>X</b>.</p>
<p>The final score of the game is sum of all the <i>m</i> counters.</p>
<p>Now Matthew needs your help to make his final score as high as possible. After that, he will show you his excellent shooting skills to get this score.</p>
<p><b>P.S.</b> Even the things above is my imagination, I hope Matthew Emmons has good luck and wins the gold metal of 50m Rifle 3*40 Men in XXX Olympics in London.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them (&lt;=50) is given in the very first line.</p>
<p>For each test case:</p>
<p>The first line contains two integers <i>n</i> and <i>m</i>. The second line contains <i>n</i> integers, the value for each bullet.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>The first and the only line contains a single integer - the highest possible final score.</p>
<h3>Example</h3>
<pre><b>Input:</b>
3
10 2
0 -1 -2 0 1 2 3 2 10 1
10 3
0 -1 -2 0 1 2 3 2 10 1
5 3
10 0 0 -1 -1

<b>Output:</b>
240
241
11

<b>Hint:</b>
For the first example, a possible solution is (0,0)(-1,-2,1,2,3,2,10,1).
For the second example, a possible solution is (0,0)(1,1)(-1,-2,2,3,2,10).
</pre>