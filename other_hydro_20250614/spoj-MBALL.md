<p>A popular event at the feline Olympics is watching and wagering on the outcome of the house cats playing Mouseball [which has the same scoring rules as American football] but is played with a catnip mouse. Wagers often involved predicting the score and, of course, some scores are more likely to occur than others. Multiples of 7 are good bets, because teams typically go for touchdowns (6 points) then attempt to kick the football between the uprights for an extra point. A score of 4 is unlikely because safeties (2 points each) are rare.</p>
<p>A score of exactly 1 is nearly (though not) impossible to achieve: suppose Team A has just scored a touchdown; during the extra point attempt, Team A fumbles the ball; it is recovered by a player from Team B, who returns it almost the entire length of the field, but fumbles right before reaching the endzone; the ball is recovered by a player from Team A, who voluntarily enters his own endzone, where he is tackled by Team B; this counts as a safety, but because it was scored during an extra point attempt, Team B will only be awarded 1 point.</p>
<p>Not surprisingly, such a scenario is not known to have ever occurred in the history of the game. So for simplicity, we will ignore this possibility altogether and consider only the following ways of scoring points:</p><ul>
<li>a safety: 2 points, always</li>
<li>a field goal: 3 points</li>
<li>a touchdown: 6 points</li>
</ul><p></p>
<p>Additionally, after scoring a touchdown, a team attempts a "try." This may be either an extra point or a two-point conversion and will give, if successful, 1 or 2 points, respectively.</p>
<p>Write a program that, given a score, outputs the number of ways that score can be achieved. As an example, a team could score 10 points in exactly 5 ways:
</p><ul>
<li>5 safeties</li>
<li>2 field goals and 2 safeties</li>
<li>a touchdown, extra point good, and a field goal</li>
<li>a touchdown, a two-point conversion, and a safety</li>
<li>a touchdown with a failed try and 2 safeties</li>
</ul><p></p>
<p>Note that order is not important: a touchdown followed by a field goal is considered equivalent to a field goal followed by a touchdown.</p>
<h3>Input</h3>
<p>The first line of input will contain an integer N &lt;= 100, indicating the number of test cases. Each of the next N lines will contain an integer S, the number of points scored by a team in a game. S will be between 0 and 100000 inclusive. (Hey, the orange &amp; blue [Flame-point Siamese] team could make it happen.)</p>
<h3>Output</h3>
<p>For each test case, output one line containing a single integer: the number of ways a team can score exactly S points.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10
6

<strong>Output:</strong>
5
3
</pre>