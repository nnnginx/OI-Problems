<p>Sheldon and Lenard are a pair of nerds playing an unimaginatively named game, "Move the books". The game board is an infinitely long strip of cells numbered 1,2,3.... from left to right. On certain cells, their favourite physics books have been placed. A player's move consists of taking any one of the books and moving it to any cell which lies to its left. But there is a constraint that you are not allowed to make your book jump over a cell that contains a book already (ie, You cannot move a book from cell j to cell i &lt; j if there is a cell k which contains one or more books such that i &lt; k &lt; j). However, you can place a book into a cell even if it contains one or more books already. But books that are placed in a cell are stacked in the order in which they arrive and hence only the topmost book (the last arrived one) can be moved from there. The players make moves alternately, and the person unable to move any book loses.</p>
<p>They have been playing the game for a long time. Sheldon makes the first move in all the games and wins most of the time. Lenard is fed up and wants to make the first move. However, Sheldon doesn't yield and this leads to an argument. This is the final agreement they have come up with:</p>
<ul>
<li> They start with N books placed in different cells. The arrangement is computer generated and hence there is no player role in this step </li>
<li> Lenard picks two natural numbers a &amp; c while Sheldon picks a natural number b. Both are unaware of the number(s) the other person has chosen while choosing their own number(s). Three more books are now added to the set : a cells to the right of the rightmost current book, b cells to the right of this book and c cells to the right of the latter book. </li>
<li> They start the game with the same rules as earlier, with Sheldon making the first move. </li>
</ul>
<p>&nbsp;</p>
<p>Now Lenard feels that there might be certain pairs (a,c) such that independent of which number Sheldon chooses, Lenard is assured to win the game. Given the initial configuration of the board find all such pairs, sort them lexicographically [(a<sub>1</sub>,c<sub>1</sub>) &lt; (a<sub>2</sub>,c<sub>2</sub>) iff a<sub>1</sub> &lt; a<sub>2</sub> or (a<sub>1</sub>=a<sub>2</sub> and c<sub>1</sub> &lt; c<sub>2</sub>)] and output the Kth such pair. If there are less than K pairs with this property, output Impossible</p>
<h3>Input</h3>
<p>The first line of the Input contains T (¡Ü50), the number of test cases. Following this are the descriptions of the T test cases</p>
<p>The first line in the description of each test case contains two space separated integers N (¡Ü1000) and K (¡Ü10<sup>8</sup>). Following these are N lines, each containing the location of a book. The book positions are given in increasing order and will each fit in a 32 bit signed integer.</p>
<h3>Output</h3>
<p>For each test case output the Kth lexicographically smallest pair of integers that will assure Lenard a win. The two integers should be separated by a space and pairs for each test case should be output on a new line. If for any test case there are less than K pairs of integers that assure Lenard a win, on the line for that test case output Impossible</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 1
1

<strong>Output:</strong>
1 1
</pre>