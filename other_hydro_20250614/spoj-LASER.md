<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">Standard mazes lose their mystery as one grows older. But throw in some lasers, and suddenly you've got yourself a recipe for cross-generational appeal. The object in any maze is to find your way from your starting point to some goal. In a&nbsp;<em>Laser Maze</em>&nbsp;you must additionally contend with laser turrets.</p>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">A laser turret is a stationary pillar that both blocks your movement and fires lasers from one side. Every time you take a step (either up, down, left, or right), every laser turret in the maze then rotates 90 degrees clockwise, and then shoots a momentary laser blast in the direction that it is facing. Needless to say, if you find yourself in the path of one of these lasers, you won't be around long enough to find a way out. A wall is a stationary pillar that blocks your movement, but does not fire lasers.</p>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">Lasers are powerful, but they do not pass through walls or laser turrets. The laser turrets respond to your movements, so you can't stand still and wait for the turrets to turn. If you reach the goal, but are immediately shot by a laser, your efforts will have been in vain, so make sure you reach the goal safely.</p>
<h3>Input</h3>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">Input begins with an integer&nbsp;<strong>T</strong>, the number of mazes you'll explore. For each maze, there is first a line containing two integers,&nbsp;<strong>M</strong>&nbsp;and&nbsp;<strong>N</strong>, the height and width of the maze, respectively. The next&nbsp;<strong>M</strong>&nbsp;lines contain&nbsp;<strong>N</strong>&nbsp;characters each, describing the maze:</p>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">. (empty space)&nbsp;<br># (wall)&nbsp;<br>S (starting position)&nbsp;<br>G (goal)&nbsp;<br>&lt; &gt; ^ v (laser turrets)&nbsp;</p>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">The four symbols for laser turrets signify turrets that are initially pointing left, right, up, or down respectively before you take your first step.</p>
<h3>Output</h3>
<p><span style="color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">For the&nbsp;</span><em>i</em><span style="color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">th maze, print a line containing "Case #</span><em>i</em><span style="color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">: " followed by the smallest number of steps necessary to get to the exit without being hit by a laser, or the string "impossible'' if there is no way to reach the goal safely.</span></p>
<h3 style="color: #141823; margin: 0px; padding: 0px; line-height: 16px;"><span style="font-size: medium;">Constraints</span></h3>
<p style="margin: 1em 0px; color: #141823; font-family: helvetica, arial, sans-serif; font-size: 12px; line-height: 16px;">1 ¡Ü&nbsp;<strong>T</strong>&nbsp;¡Ü 100&nbsp;<br>1 ¡Ü&nbsp;<strong>M</strong>,&nbsp;<strong>N</strong>&nbsp;¡Ü 100&nbsp;<br>Each maze will contain exactly one 'S' and exactly one 'G'.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="margin: 0px; color: #141823; font-size: 12px; line-height: 16.08px;">5
2 5
##^##
S...G
2 5
##v##
S...G
1 5
S..G&lt;
1 6
S...G&lt;
5 5
S....
.....
.&gt;v..
.^&lt;..
....G</pre>
<strong>Output:</strong>
<pre style="margin: 0px; color: #141823; font-size: 12px; line-height: 16.08px;">Case #1: 6
Case #2: 4
Case #3: 3
Case #4: impossible
Case #5: 8</pre>
</pre>