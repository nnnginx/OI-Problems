<p>In this problem you need to assist in computing the probability of winning at tennis. Here is a brief explanation of how the scoring system works. In a tennis <em>match</em>, players play a certain number of consecutive <em>sets</em>. Each <em>set</em> is in turn made up of a series of <em>games</em> (and may include a <em>tie-break</em> if needed). Finally each game is made of <em>points</em>.</p>
<!--TOC paragraph Points.-->
<h5 class="paragraph"><!--SEC ANCHOR -->Points.</h5>
<!--SEC END -->
<p>Every point is started by one of the players serving (i.e.&nbsp;hitting the ball into the service box in the opposite court) and the other receiving serve. The server then attempts to return the ball into the server’s court and players alternate hitting the ball across the net. When one of the players fails to make a legal return (e.g. if the ball is knocked out of the court), he or she loses the point. The specifics of how points are won are not important to us.</p>
<!--TOC paragraph Games.-->
<h5 class="paragraph"><!--SEC ANCHOR -->Games.</h5>
<!--SEC END -->
<p>The scoring system within a game is peculiar to say the least. As the player wins points in a game, his score goes from the initial value of 0 (read “love”) to 15, 30, or 40 (yes, just when you think you’re starting to spot a pattern in this mess it breaks down). There is no a-priori limit to the length of a game (meaning the number of points played), but a player’s score is always indicated by one of these numbers according to the following rules. When a player has three points (score 40) and wins the following point as well, he wins the game unless the scoreline was 40−40 (read “deuce”) to start with. A player needs to win two consecutive points from deuce to win the game. Winning one gives him advantage; if followed by a second winning point the game is won by him, but if followed by a losing point the score reverts to deuce.</p>
<p>Example: at 40−30, if the first player wins the next point he wins the game. However, if the second player wins the next three points the game is his.</p>
<!--TOC paragraph Sets.-->
<h5 class="paragraph"><!--SEC ANCHOR -->Sets.</h5>
<!--SEC END -->
<p>A player wins a set if he wins at least six games (in the current set) and he is two games ahead of his opponent but, as you may be starting to suspect, there is yet another exception. In case the scoreline for the number of games won reaches six-all (6−6), a tie-break is played instead to decide the set.</p>
<p>Example: at 5−4, if the first player wins the next game he takes the set 6−4. But if he loses, the set is still undecided and can eventually go to either 7−5, 5−7 or a tie-break.</p>
<!--TOC paragraph Tie-break.-->
<h5 class="paragraph"><!--SEC ANCHOR -->Tie-break.</h5>
<!--SEC END -->
<p>A tie-break (and the set to which it belongs) is won when a player wins at least seven points by a margin of two points or more.</p>
<!--TOC paragraph Match.-->
<h5 class="paragraph"><!--SEC ANCHOR -->Match.</h5>
<!--SEC END -->
<p>The winner of a match is the first player to win 2 sets (the wins do not need to be consecutive). Hence a match may go to 2 or 3 sets depending on how the game develops.</p>
<p><br> Rafa has been carefully studying his past performances against his next opponent and he knows he wins each point with probability precisely <em>p</em>, irrespective of whether he is serving or receiving and regardless of all other points played. Can you help him assess his chances of winning the match?</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case is described by a single floating point number <em>p</em>, 0 ≤ <em>p</em> ≤ 1 in its own line. A value of −1 for <em>p</em> marks the end of the input.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, print a single line with the probabilities of Rafa winning a given game, set and match, respectively. These three numbers must be separated by a space character. Your answers should be accurate to within an absolute error of 10<sup>−6</sup>.</p>
<p><br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">0.5
0.3
0.7
-1
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">0.50000000000 0.50000000000 0.50000000000
0.09921103448 0.00016770463 0.00000008437
0.90078896552 0.99983229537 0.99999991563
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David García Soriano</em></blockquote>