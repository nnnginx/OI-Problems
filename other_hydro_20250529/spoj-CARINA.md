<p>Little Petar had played the Flappy Bird game for far too long, and got bored of the fact that the bird never gets tired and always jumps with the same intensity. As this felt very unnatural, he had decided to make his own version of the game, dubbed PetarVBird™. However, he was immediately reported to the police for violating intellectual property laws, and as such his options for distributing the game abroad are very limited.</p>
<p>Petar made a specific number of copies of the game, and intends to transport them from the company (location A) to the distributer (location B). To do this, he has in his possession a single truck, capable of carrying a limited amount of copies at once. Along the way from A to B there is a series of customs checkpoints; if Petar is carrying at least one copy of the game in his truck at the moment of arrival to the checkpoint, he is obliged to give a copy to the customs officers as a bribe. It is possible to unload the copies at the checkpoint, and then load them back in again. In addition, to avoid making the traffic police suspicious, Petar does not want to return back to location A more than X times.</p>
<p>Petar is interested in the maximal amount of copies of the game he can successfully deliver to location B, under these constraints.</p>
<h3>Input</h3>
<p>The first and only line of the standard input contains four integers: N, C, L and X, representing the number of copies, the truck's capacity, the number of checkpoints between A and B and the maximal amount of returns to A allowed, respectively.</p>
<h3>Output</h3>
<p>Write to the first and only line of the standard output a single integer, representing the maximal amount of copies of the game that can be delivered to location B.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4000 1000 1000 1</pre>
<pre><strong>Output:</strong>
500
</pre>
<h3>Explanation</h3>
<p>Petar may first load up his truck with 1000 copies, drive them to the 500th checkpoint along the way, and unload the 500 copies he has left. After that he returns to A and does the same thing again. Now there are 1000 copies at the 500th checkpoint, which Petar will all collect and carry on to B, with 500 copies delivered. There is no strategy that will result in more copies successfully delivered to B.</p>
<h3>Constraints</h3>
<ul>
<li>1 &lt;= N, C, L &lt;= 10<sup>18</sup></li>
<li>0 &lt;= X &lt;= 10<sup>6</sup></li>
</ul>