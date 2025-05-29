<p>The inhabitants of a small Caribbean island in the region known as Bermuda¡¯s Triangle love to
spend their warm summer nights playing cards. As a tribute to the region where they live, all
of their card games have some connection to triangles. One of the most popular games in the
island is known as Triples, and has very simple rules.

</p><p></p><p>
The game is played between two players, with a set of standard playing cards. Cards are
distinguished only by their values, from 1 (Ace) to 13 (King). The cards are shuffled and
placed as a pile in the center of the table, face down. This pile is called the stock. The two
players take turns at playing. At each turn, a player
</p><p></p><p>

</p><ul>
<li> draws the top card from the stock, adding it to her/his hand; and
<p></p><p>
</p></li><li> decides whether she/he wants to ¡°drop some triples¡±.
</li></ul>

<p></p><p>
Dropping a triple consists of choosing three cards (a <i>triple</i>) from the hand and placing them
on the table, face up. The dropped triples stay on the table until the end of the game. Only
some sets of three cards form a valid triple. There are two types of valid triples:

</p><p></p><p>
</p><ul>
<li> Perfect triples are made of three cards whose values represent the length of sides of an
equilateral triangle;

<p></p><p>
</p></li><li> Common triples are made by three cards whose values represent the length of sides of
any other (not equilateral) triangle.
</li></ul>

<p></p><p>
The figure below shows examples of perfect triples (a), common triples (b), and invalid triples
(c).

</p><p></p><p>
</p><center><img src="/content/steinersp:triples.jpg" alt="subir imagenes" border="0"></center>

<p></p><p>
Only valid triples can be dropped, but a player may drop any number of triples at a given
turn. In particular, since players know the number of cards in the stock at every turn, a player
may decide to drop all triples in her/his last turn. Some players, however, normally drop some
triples during the game, to maintain as few cards in their hands as possible.

</p><p></p><p>
The game finishes when the stock is empty. The winner is the player that dropped the largest
number of perfect triples. If both players dropped the same number of perfect triples, the winner is the player that dropped the largest number of common triples. If both players dropped the
same number of perfect triples and the same number of common triples, the result is a tie.

</p><p></p><p>
Given the description of the cards in the stock, write a program that determines the winner of
a game of Triples, considering both players play as best as possible.

</p><h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains one integer N
representing the number of cards in the stock (6 &lt;= N &lt;= 10<sup>4</sup>). The next line contains N
integers X<sub>i</sub>, separated by single spaces, representing the cards in the stock (1 &lt;= X<sub>i</sub> &lt;= 13, for
1 &lt;= i &lt;= N). The cards are given in the order they are drawn by the players: the first card
in the input (X<sub>1</sub>) is the first card drawn, the second card in the input (X<sub>2</sub>) is the second card
drawn, and so on. Several cards with the same value may be present in the stock, and not
necessarily all card values are present in the stock. The end of input is indicated by N = 0.

</p><h3>Output</h3>
<p>For each test case your program must output a single line, containing ¡®1¡¯ if the first player to
play wins the game, ¡®2¡¯ if the second player wins, or ¡®0¡¯ if there is a tie.

</p><h3>Example</h3>

<pre><b>Input:</b>
7
5 6 5 6 5 6 8
12
13 13 13 13 13 13 1 3 2 9 3 9
12
1 2 1 2 1 2 3 1 4 2 5 3
0

<b>Output:</b>
0
2
1
</pre>