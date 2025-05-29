<p>On a hot day in Surabaya, Puguh is bored. He then declares himself as "the bestest player in teh wurld", challenging his friend named Joke to play a game. Here is the description of the game:</p>
<ul>
<li>There are N piles of coins and each pile contains Xi&nbsp;coins (i=1 to N).</li>
<li>Each player alternately takes turn.</li>
<li>On each turn, a player must take a number of coin from any pile. The number of coin taken must be a divisor of the current pile size and must be less than the current pile size. For example, if Puguh chooses a pile with 6 coins, then he may take 1, 2, or 3 coins from that pile.</li>
<li>The first player that can't take any coin on his turn loses.</li>
</ul>
<p>Puguh and Joke will play optimally. If Puguh is the first player to move, predict the winner of this game.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Input starts with a number T, the number of test cases. For each test case, the first line contains a number N. The next line contains N numbers Xi, number of coins on the i-th pile.</p>
<h3>Output</h3>
<p>For each case, output a line. If Puguh won the game, output "Puguh is the bestest player in teh wurld" and if Joke won the game, output &nbsp;"Joke is the bestest player in teh wurld".</p>
<h3>Sample Input</h3>
<pre>1 <br>1 <br>6</pre>
<h3>Sample Output</h3>
<pre>Puguh is the bestest player in teh wurld</pre>
<div style="border: 1px solid #FC0; background-color: #ffc; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<ul>
<li>1 ¡Ü T ¡Ü 50</li>
<li>0 ¡Ü N ¡Ü 100000</li>
<li>0 ¡Ü Xi ¡Ü 1000000000</li>
</ul>
</div>
<p><span style="font-weight: bold;">Input file is huge, use faster I/O (scanf for C)</span></p>