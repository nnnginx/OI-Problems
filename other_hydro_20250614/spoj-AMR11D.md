<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are the organizer of a Wizarding Duel tournament at Hogwarts. N players participated in the tournament and each player played with every other player exactly once, and each such game resulted in a winner and a loser (no drawn games). It is now time to declare the results. Each player's score is the number of games the player won. However, you realize that something possibly went wrong with the scoring system, and the scores that you have noted down might be wrong. In fact, the scores you have noted down could simply not be possible. For example, suppose there are 3 players and the scores that you noted are 0,0 and 2. Clearly this is not possible as the game between the first two players must have had a winner and thus both the players cannot have score 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">While you have no way to figure out the correct scores of each player, you've decided to set the scores right by adjusting the scores of some players. The new set of scores should be possible to have arisen in the tournament, otherwise there would be ample proof that the scoring is wrong. However, making drastic changes might cause suspicion. So you've decided to adjust the scores so that the sum of the absolute differences between the old and the new scores of each player is minimized. In other words, if the original scores which you noted are a1,..,aN, you must change them to the series of possible scores b1,...bN such that the sum |ai - bi| is minimized.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow. Each case contains an integer N on the first line, followed by the set of scores which you have noted down: a1..aN.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one for each test case, containing the minimum sum of absolute values in order to make the scorecard a valid one.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 20</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 &lt;= N &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 &lt;= ai &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: 3 seconds</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 64 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 0 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5 3 2 1 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<p>&nbsp;</p>
<p>You are the organizer of a Wizarding Duel tournament at Hogwarts. N players participated in the tournament and each player played with every other player exactly once, and each such game resulted in a winner and a loser (no drawn games). It is now time to declare the results. Each player's score is the number of games the player won. However, you realize that something possibly went wrong with the scoring system, and the scores that you have noted down might be wrong. In fact, the scores you have noted down could simply not be possible. For example, suppose there are 3 players and the scores that you noted are 0,0 and 2. Clearly this is not possible as the game between the first two players must have had a winner and thus both the players cannot have score 0.</p>
<p>&nbsp;</p>
<p>While you have no way to figure out the correct scores of each player, you've decided to set the scores right by adjusting the scores of some players. The new set of scores should be possible to have arisen in the tournament, otherwise there would be ample proof that the scoring is wrong. However, making drastic changes might cause suspicion. So you've decided to adjust the scores so that the sum of the absolute differences between the old and the new scores of each player is minimized. In other words, if the original scores which you noted are a1,..,aN, you must change them to the series of possible scores b1,...bN such that the sum |ai - bi| is minimized.</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T. T test cases follow. Each case contains an integer N on the first line, followed by the set of scores which you have noted down: a1..aN.</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output T lines, one for each test case, containing the minimum sum of absolute values in order to make the scorecard a valid one.</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 20</p>
<p>2 &lt;= N &lt;= 50</p>
<p>0 &lt;= ai &lt;= 100</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3</p>
<p>0 0 2</p>
<p>5</p>
<p>5 3 2 1 4</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>1</p>
<p>5</p>
<p>&nbsp;</p>
<p>&nbsp;</p>