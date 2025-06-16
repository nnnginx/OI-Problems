<div style="text-align: left; margin: 10px 0px;"><div style="float: right; margin: 0px 0px 3px 10px;"><img src="/content/crazyb0y:FNINJA.jpg" width="250"></div><span>

<blockquote>
<i><p>Fruit Ninja is a juicy action game enjoyed by millions of players around the world, with squishy, splat and satisfying fruit carnage! Become the ultimate bringer of sweet, tasty destruction with every slash.</p>
<p>--- Wikipedia</p>
</i>
</blockquote>
</span></div>

<p>It is a very popular game on cell phones where people can enjoy cutting the fruit by touching the screen. The screen is rectangular, and all the fruit can be considered as circles, with coordinate of the center, and radius. Note that the fruit may overlap with each other. In this problem, a touch is a straight line cutting through the whole screen, scoring all the fruits it cuts or touches.</p>

<p>Now Fred is playing the Fruit Ninja, and seems absorbed in the game. He's desperate to create a new record, so he asks you for help. Now you are given a screen shot of the game, help him find the highest score he can get in a single touch.</p>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 50), indicating the number of test cases.</p>

<p>Each test case contains several lines.
The first line contains an integer <b>N</b> (1 �� <b>N</b> �� 1000), indicating the number of fruit.</p>

<p>The following <b>N</b> lines each contains three integers <b>X</b><sub>i</sub>, <b>Y</b><sub>i</sub>, <b>R</b><sub>i</sub> (-1000 �� <b>X</b>, <b>Y</b> �� 1000, 1 �� <b>R</b><sub>i</sub> �� 1000), representing a fruit on the screen, where (<b>X</b>, <b>Y</b>) is the coordinate of the center of the fruit, and <b>R</b><sub>i</sub> is the radius.</p>

<p>You can assume the screen is infinite.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is maximum number of fruit that you can cut in a single touch.</p>

<p>It is guaranteed that the answer will remain the same even if you expand the radius of all the fruit slightly by 10<sup>-5</sup>.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4
-2 5 1
5 5 1
-3 2 1
0 1 1
4
-4 5 1
3 2 1
-5 3 1
4 -3 1

<b>Output:</b>
Case #1: 3
Case #2: 2
</pre>