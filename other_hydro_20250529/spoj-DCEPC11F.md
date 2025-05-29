<p>Kapish is a huge fan of football. He loves anything and everything related to the game and never misses a single match when his favourite team, Manchester United, is playing. Being the coder that he is, one day he decides to create his own, slightly modified version of football, through code.</p>
<p>The game is played between 2 teams having <strong>M players</strong> each and continues for <strong>N minutes</strong>. In each minute of the game, <strong>exactly one</strong> of the following 5 events will take place:</p>
<ol>
<li>Team 1 scores a goal</li>
<li>Team 2 scores a goal</li>
<li>A player from team 1 gets a red card</li>
<li>A player from team 2 gets a red card</li>
<li>None of the above</li>
</ol>
<p>A player who gets a red card can take no further part in the game. If at any point of time, a team is left with less than 5 players on the field, it will automatically get disqualified, and the other team will be declared as the winner.</p>
<p>Kapish is very pleased with his new game. However, Pushap, who hates boring draws in football, is not impressed. ¡°Do you even know how many ways are there for this game to end in a draw?¡± he asks.</p>
<p>Given N and M, can you help Kapish find out the number of ways for the game to end in a draw? (draw means both teams end up with the same number of goals at the end of N minutes) Since the number of ways can be very large, you need to print the answer mod 1000000007.</p>
<p>Note 1: Two ways are considered different, if the event(s) of at least 1 minute are different in them.</p>
<p>Note 2: For the sake of simplicity, you can assume that all the players in a team are identical.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases.</p>
<p>Each test case consists of a single line, with 2 space separated integers, N and M.</p>
<h3>Output</h3>
<p>For each test case, output a single line, containing the number of ways mod 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>1 11</pre>
<pre>2 8
</pre>
<pre><strong>Output:</strong>
3</pre>
<pre>11</pre>
<pre><p>Explanation: In the first test case, in the first minute, the occurrence of any of the events 3, 4 and 5 described in&nbsp;</p><p>the problem can lead to a draw. Hence there are 3 ways for it to end in a draw.</p><h3>Constraints</h3><p>1&lt;=T&lt;=100</p><p>5 &lt;= M &lt;= 11</p><p>1 &lt;= N &lt;= 100</p></pre>