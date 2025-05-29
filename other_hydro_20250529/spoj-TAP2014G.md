<p><strong>[ The original version of this problem (in Spanish) can be found at&nbsp;</strong><strong><a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a></strong><strong>&nbsp;]</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Every weekend, Germ¨¢n and Gianina play a football match with their friends. This Saturday, both German and Gianina are injured, so they will participate in the game as coaches.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">To choose the teams they will use the following procedure: of the N friends they have, each of them is going to pick N/2 players (N is even), the selection process is going to take N/2 turns. On every turn, each of them chooses a different player from the ones who have not been selected yet, and this player is assigned to his/her team. Germ¨¢n won the coin flip and he gets to choose first on every turn. However, to be gallant, Germ¨¢n can let Gianina go first on some turns if he wants so.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, if N = 6 there are N/2 = 3 turns. Suppose Germ¨¢n decides to yield his right to choose first on the second and third turn, but not on the first one. In that case, the order of selection of players would be:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">[Formula / Figure]</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">As we all know, football is a sport ruled by logic. Every friend of Germ¨¢n and Gianina has a score that indicates how well they play. If the sum of scores of Germ¨¢n's team is strictly greater than the sum of scores of Gianina's team, then Germ¨¢n's team will win the match. If the sum of scores is the same for both teams, the match ends in a draw. Otherwise, Gianina's team will be the winner.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Germ¨¢n wants to be gallant, but he is more interested on winning the game. He wants to yield his turn as many times as possible so that he can win the game anyway. Gianina also wants to win the game, therefore each time they choose a player they will do it in a way that maximizes their chances of winning.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains an integer N with the number of players to choose from (with 2 &lt;= N &lt;= 1000, N is even). The second line contains N integers P_1, P_2, ... , P_N representing the scores of each player (1 &lt;= P_i &lt;= 1000 for i = 1, 2,..., N).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Print a line containing a single integer that represents how many times Germ¨¢n can yield his turn in such a way that his team's victory is guaranteed. If Germ¨¢n can not ensure a victory, you must print the number -1.</div>
<p>Every weekend, Germ¨¢n and Gianina play a football match with their friends. This Saturday, both German and Gianina are injured, so they will participate in the game as coaches.</p>
<p>To choose the teams they will use the following procedure: of the <strong>N</strong> friends they have in common, each of them is going to pick <strong>N/2</strong> players (<strong>N</strong> is even), with the selection process taking&nbsp;<strong>N/2</strong> turns. On every turn, each of them chooses a different player among the ones who have not been selected yet, and this player is assigned to his/her team. Germ¨¢n won the initial coin flip so he gets to choose first on every turn. However, to be gallant Germ¨¢n can let Gianina go first on some turns if he wants so.</p>
<p>For example, if <strong>N = 6</strong> there are <strong>N/2 = 3</strong> turns. Suppose Germ¨¢n decides to yield his right to choose first on the second and third turns, but not on the first one. In that case, the order of selection of players would be:</p>
<p style="text-align: center;"><strong>Germ¨¢n - Gianina || Gianina &nbsp;- Germ¨¢n || Gianina &nbsp;- Germ¨¢n</strong></p>
<p style="text-align: center;"><strong>&nbsp;</strong><span style="font-weight: bold;">Turn 1 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Turn 2 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Turn 3</span></p>
<p>As we all know, football is a sport ruled by logic. Every friend of Germ¨¢n and Gianina has a score that indicates how well they play. If the sum of scores of Germ¨¢n's team is strictly greater than the sum of scores of Gianina's team, then Germ¨¢n's team will win the match. If the sum of scores is the same for both teams, the match ends in a draw. Otherwise, Gianina's team will be the winner.</p>
<p>Germ¨¢n wants to be gallant, but he is even more interested in winning the game. Therefore, he wants to yield his turn as many times as possible so that he can still win the game anyway. Gianina also wants to win the game, therefore each time they choose a player they will both do it in a way that maximizes their chances of winning.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>N</strong> representing the number of players to choose from (with <strong>2 ¡Ü&nbsp;N&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;1000</strong>&nbsp;and&nbsp;<strong>N</strong> even). The second line contains <strong>N</strong> integers <strong>P<sub>1</sub>, P<sub>2</sub>, ..., P<sub>N</sub></strong> representing the scores of each player (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;P<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;1000</strong>&nbsp;for <strong>i = 1, 2, ..., N</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a line containing a single integer that represents how many times Germ¨¢n can yield his turn in such a way that his team's victory is guaranteed. If Germ¨¢n can not ensure a victory, you must print the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">6
7 8 2 10 1 4</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">6
7 8 2 10 1 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">2</span></pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
60 95 100 65</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">0</span></pre>
<h3>Example 4</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">10
10 10 10 10 10 10 10 10 10 10</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">-1</span></pre>