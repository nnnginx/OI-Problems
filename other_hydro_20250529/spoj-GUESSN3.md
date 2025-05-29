<h3>GUESSN3</h3>
<p>Judge has chosen an integer x in the range [1, n]. Your task is to find x, using query as described below. But be careful, because the Judge can lie. Judge is allowed to lie only once in single game and only in reply for query.</p>
<h3>Query</h3>
<p>Single query should contains range R = [a, b]. The reply for query is "YES", if a �� x �� b. Otherwise the reply is "NO".</p>
<p>1 �� a �� b �� n</p>
<h3>Communication</h3>
<p>You should communicate with Judge using standard input and output.</p>
<p><em><strong>Attention: the program should clear the output buffer after printing each line. It can be done using fflush(stdout) command or by setting the proper type of buffering at the beginning of the execution - setlinebuf(stdout).</strong></em></p>
<p>The first line of input contains single integer T, the number of games. Then T games follow.</p>
<p>At the beggining of each game You should send to the Judge a line with command "START_GAME". The Judge will answer You with numbers n, m, where n is as described above&nbsp;and m&nbsp;is the maximum number of queries that You can use in this game.</p>
<p>Then You should send some queries, every query is a line with "QUERY" keyword, then single-space separated values a b. After each query the Judge will answer "YES" or "NO".</p>
<p>At the end of game You should give answer: "ANSWER y", where 1 �� y �� n is the answer for the game. When y ��&nbsp;x, the solution will got WA.</p>
<p>Then start the next game (if there is any).</p>
<h3>Constraints</h3>
<p>1 �� T �� 2<sup>10</sup></p>
<p>2 �� n �� 10<sup>18</sup></p>
<p>m: This value will be as small as possible. This means, that there exists strategy for player to find the value x using m queries, but there doesn't exist such strategy using m-1 queries.</p>
<h3>Example</h3>
<p>The example of communication. J=Judge, P=Player.</p>
<p>J: 3</p>
<p>P: START_GAME<br> J: 2 3</p>
<p>P: QUERY 1 1<br> J: YES<br> P: QUERY 2 2<br> J: YES<br> P: QUERY 1 1<br> J: NO<br> P: ANSWER 2</p>
<p>P: START_GAME<br> J: 2 3</p>
<p>P: QUERY 1 1<br> J: YES<br> P: QUERY 2 2<br> J: NO<br> P: ANSWER 1</p>
<p>P: START_GAME<br> J: 5 6</p>
<p>P: QUERY 1 3<br> J: YES<br> P: QUERY 4 5<br> J: YES<br> P: QUERY 2 4<br> J: YES<br> P: QUERY 3 4<br> J: NO<br> P: ANSWER 2</p>
<p>Explanation:</p>
<p>In 1st game there is conflicting information in first and second query, so we know, that the last query isn't lie.</p>
<p>In 2nd game the Judge don't use lie (Judge can lie once, but don't need to do it).</p>
<p>In 3rd game there is conflicting information in first and second query, so the next queries has correct answers.</p>
<h3>Note</h3>
<p>Be careful. The Judge will try to maximize the number of queries that You will ask. If necessary, the Jugde can also replace chosen value x with the other one. But don't worry too much - at the end of the game, the value x chosen by Judge will satisfy all except at most one of Your queries.</p>
<h3>Similar problems</h3>
<p>There is a family of similar problems. Here is the table with them:</p>
<table border="1">
<tbody>
<tr>
<th>Code</th><th>Number of lies</th><th>Query format</th><th>Type</th><th>Section</th><th>Difficulty</th>
</tr>
<tr>
<td><a href="../../problems/GUESSN1/">GUESSN1</a></td>
<td>1</td>
<td>subset</td>
<td>interactive</td>
<td>challenge</td>
<td>easy</td>
</tr>
<tr>
<td><a href="../../problems/GUESSN2/">GUESSN2</a></td>
<td>2-16</td>
<td>subset</td>
<td>interactive</td>
<td>challenge</td>
<td>medium/hard</td>
</tr>
<tr>
<td><a href="../../problems/GUESSN3/">GUESSN3</a></td>
<td>1</td>
<td>range</td>
<td>interactive</td>
<td>classical</td>
<td>medium</td>
</tr>
<tr>
<td><a href="../../problems/GUESSN4/">GUESSN4</a></td>
<td>1</td>
<td>subset</td>
<td>non-interactive</td>
<td>challenge</td>
<td>medium</td>
</tr>
<tr>
<td><a href="../../problems/GUESSN5/">GUESSN5</a></td>
<td>2-16</td>
<td>subset</td>
<td>non-interactive</td>
<td>challenge</td>
<td>hard</td>
</tr>
</tbody>
</table>
<p>subset - the query is about any subset of {1,2,...,n}<br> range - the query is about any range [a,b]<br>&nbsp;interactive - the Judge replies after every query<br> non-interactive - all queries have to be asked at once, before any reply</p>