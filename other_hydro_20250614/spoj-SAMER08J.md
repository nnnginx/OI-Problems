<p>Bora Bora is a simple card game for children, invented in the South Pacific Island of the same name. Two or more players can play, using a deck of standard cards. Cards have the usual ranks: Ace, 2, 3, 4, 5, 6, 7, 8, 9, 10, Jack, Queen and King. Each card has also one of four suits: Clubs, Diamonds, Hearts and Spades.</p>
<p>Players sit on a circle around the table and play by turns.  The next player to play may be the one to the left (clockwise direction) or to the right (counter-clockwise direction) of the current player, depending on the cards played, as we will see. At the start, the direction of play is clockwise.</p>
<p>The deck is shuffled and each player is dealt a hand of cards. The remaining of the deck is placed, face down, on the table; this is called the <em>stock</em> pile.  Then the first (topmost) card is removed from the stock and placed on the table, face up, starting another pile, called the <em>discard</em> pile.</p>
<p>The objective of the game is for a player to discard all his cards. At each turn, a player discards at most one card. A card can be discarded only if it has the same rank or the same suit as the topmost card on the discard pile. A player discards a card by placing it, face up, in the discard pile (this card becomes the topmost). If a player does not have a suitable card to discard on his turn, he must draw one card from the stock and add it to his hand; if he can discard that card, he does so, otherwise he does nothing else and his turn ends.  A player always discards the highest valued card he possibly can. The <em>value</em> of a card is determined first by the card rank and then by the card suit. The rank order is the rank itself (Ace is the lowest, King is the highest), and the suit order is, from lowest to highest, Clubs, Diamonds, Hearts and Spades. Therefore, the highest valued card is the King of Spades and the lowest valued card is the Ace of Clubs. As an example, a Queen of Diamonds has a higher value than a Jack (any suit) but has a lower value than a Queen of Hearts.</p>
<p>Some of the discarded cards affect the play, as follows:</p>
<p>&nbsp;</p>
<ul>
<li> when a Queen is discarded, the direction of play is reversed: if   the direction is clockwise, it changes to counter-clockwise, and   vice-versa;<br><br></li>
<li> when a Seven is discarded, the next player to play must draw two   cards from the stock (the number of cards in his hand   increases by two), and misses his turn (does not discard any   card);<br><br></li>
<li> when an Ace is discarded, the next player to play must draw one   card from the stock (the number of cards in his hand increases   by one), and misses his turn (does not discard any card);<br><br></li>
<li> when a Jack is discarded, the next player to play misses his turn   (does not discard any card).<br><br></li>
</ul>
<p>Notice that the penalty for the first card in the discard pile (the card draw from the stock at the beginning) is applied to the first player to play. For example, if the first player to play is <em>p</em> and the first card on the discard pile is an Ace, player <em>p</em> draws a card from the stock and does not discard any card on his first turn.  Also notice that if the first card is a Queen, the direction of play is reversed to counter-clockwise, but the first player to play remains the same.</p>
<p>The winner is the player who first discards all his cards (the game ends after the winner discards his last card).</p>
<p>Given the description of the shuffled deck and the number of players, write a program to determine who will win the game.</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains three integers <em>P</em>, <em>M</em> and <em>N</em>, separated by single spaces, indicating respectively the number of players (2   �� <em>P</em> �� 10), the number of cards distributed to each of the players at the beginning of the game (1   �� <em>M</em> �� 11) and the total number of cards in the shuffled deck (3   �� <em>N</em> �� 300). Each of the next <em>N</em> lines contains the description of one card.  A card is described by one integer <em>X</em> and one character <em>S</em>, separated by one space, representing respectively the card rank and the card suite. Card ranks are mapped to integers from 1 to 13 (Ace is 1, Jack is 11, Queen is 12 and King is 13).  Card suits are designated by the suit's first letter: '<tt>C</tt>' (Clubs), '<tt>D</tt>' (Diamonds), '<tt>H</tt>' (Hearts) or '<tt>S</tt>' (Spades).</p>
<p>Players are identified by numbers from 1 to <em>P</em>, and sit on a circle, in clockwise direction, 1, 2  ��<em>P</em>, 1. The first <em>P</em>��<em>M</em> cards of the deck are dealt to the players: the first <em>M</em> cards to the first player (player 1), the next <em>M</em> to the second player (player 2), and so on. After dealing the cards to the players, the next card on the deck - the (<em>P</em> ��<em>M</em> + 1)-th card - is used to start the discard pile, and the remaining cards form the stock. The (<em>P</em> ��<em>M</em> + 2)-th card to appear on the input is the topmost card on the stock, and the last card to appear on the input (the <em>N</em>-th card) is the bottommost card of the stock (the last card that can be drawn). Player 1 is always the first to play (even when the card used to start the discard pile is a Queen). All test cases have one winner, and in all test cases the number of cards in the deck is sufficient for playing to the end of the game.</p>
<p>The end of input is indicated by a line containing only three zeros, separated by single spaces.</p>
<h3>Output</h3>
<p>For each test case in the input, your program must print a single line, containing the number of the player who wins the game.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2 10
1 D
7 D
1 S
3 C
13 D
1 S
5 H
12 D
7 S
2 C
3 2 11
1 S
7 D
11 D
3 D
7 D
3 S
11 C
8 C
9 H
6 H
9 S
3 3 16
1 H
10 C
13 D
7 C
10 H
2 S
2 C
10 S
8 S
12 H
11 C
1 C
1 C
4 S
5 D
6 S
0 0 0


<strong>Output:</strong>
1
3
2

</pre>