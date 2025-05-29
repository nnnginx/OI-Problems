<p>Gon is on Greedy island. He wants to go home. But to get the ticket to leave the game, he has to get N cards labeled in a sequence from 1 to N (the order of the cards in his hand is irrelevant). He already has N cards, but not forming a sequence from 1 to N. So he wants you to help him. For some cards, he can change one card for another for one piece of gold. Help him to get the ticket at the minimum cost (using the minimum number of exchanges).

</p><h3>Input</h3>
<p>
The first line contains t, the number of tests (1&lt;=t&lt;=10). For each test case:
</p><ul>
<li>the number of cards N is given is given in the first line (2&lt;=N&lt;=500).
</li><li>the next N lines contain the N cards owned by Gon.
</li><li>the following line contains e, the number of different allowed types of exchanges.
</li><li>the next e lines contain two integers x<sub>i</sub>,y<sub>i</sub> each which mean that we can exchange and replace the card marked x by the card marked y and vice versa.
</li></ul>
<p>There is a blank line after each test case.

</p><h3>Output</h3>
<p>
For each test case, output a line denoting the minimum required cost.
</p><h3>Example</h3>
<pre><b>Input:</b>
1
4
1
2
2
2
2
2 3
3 4

<b>Output:</b>
3
</pre>