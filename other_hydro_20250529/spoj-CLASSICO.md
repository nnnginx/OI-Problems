<!--Converted with LaTeX2HTML 2008 (1.71) original version by:  Nikos Drakos, CBLU, University of Leeds * revised and updated by:  Marcus Hennecke, Ross Moore, Herb Swan * with significant contributions from:   Jens Lippmann, Marek Rouchal, Martin Wilck and others -->
<p>The <span class="textit">Old Yellers</span>, the contestants of the old days of IIUC are going to have a football match with the current contestants. As the <span class="textit">yellers</span> are going to be the host of the match, it will be called 'Yell Classico'. As the yellers are always busy in yelling, oops, I mean programming, they have appointed you as the manager of their team. Now, as a manager of the <span class="textit">Yeller</span> team, you have to select 11 players for the match from <span class="MATH"><em>N</em></span> players.</p>
<p>All the <span class="MATH"><em>N</em></span> players will stand in a line just before the match. Your task will be to select 11 players from them in such a way that, the player standing in front is as tall as possible. If there are more than one such team formations, do it in a way where the 2nd player is as tall as possible. If still there is a tie, choose the formation having tallest player in the 3rd position and so on. (<span class="textbf">Which means, until you can break the tie or reach the 11th position, keep looking in the next position</span>).</p>
<p>Note that,</p>
<ol>
<li>You don't have enough time to change the order in which players are standing. </li>
<li>If you have tie even after reaching the 11th position, select from any of the tied formations. </li>
</ol>
<p>Players are quite same in their playing abilities, you don't need to bother about that.</p>
<h4 style="font-size: 10px;"><span style="color: #ff0000;"><span style="font-size: small;">Input</span></span></h4>
<p>First line of input will contain the number of test cases, <span class="MATH"><em>T&lt;</em>100</span>.</p>
<p>For each test case, there are two lines.</p>
<p>The first line contain <span class="MATH"><em>N</em></span> (number of players, <!-- MATH  $1 \le N \le 2000$  --> <span class="MATH">1&lt;<em>N&lt;</em>2000</span>).</p>
<p>The second one is a line of <span class="MATH"><em>N</em></span> integers separated by spaces. The ith integer of this line will specify the height of the ith player. (Heights will not be greater than <span class="MATH">10<sup>9</sup></span>).</p>
<h4 style="font-size: 10px;"><span style="color: #ff0000;"><span style="font-size: small;">Output</span></span></h4>
<p>For each test case output `<tt>Case <span class="MATH"><em>X</em></span>: </tt>', (<span class="MATH"><em>X</em></span> is the case number, starting from 1). Then print the heights of the 11 selected players separated by spaces. If it's not possible to select exactly 11 players, then send the spectators home by printing `<tt>go home!</tt>' (Without quotations). See the sample output for exact formatting.</p>
<h4 style="font-size: 10px;"><span style="color: #ff0000;"><span style="font-size: small;">Sample Input</span></span></h4>
<pre>4
15
2 10 8 5 1 5 9 9 3 5 6 6 2 2 8
11
2 6 3 8 7 2 5 3 4 3 3
4
2 7 9 6
12
6 2 3 8 7 2 5 3 4 3 3 10</pre>
<h4 style="font-size: 10px;"><span style="color: #ff0000;"><span style="font-size: small;">Output for Sample Input</span></span></h4>
<pre>Case 1: 10 8 9 9 3 5 6 6 2 2 8
Case 2: 2 6 3 8 7 2 5 3 4 3 3
Case 3: go home!
Case 4: 6 3 8 7 2 5 3 4 3 3 10</pre>
<pre></pre>
<p><strong><span style="font-size: small;"><span class="textbf">Problem Setter:</span>&nbsp;Bidhan Roy</span></strong></p>
<hr>