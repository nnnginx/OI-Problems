<p><img style="float:right; margin-left:50px; margin-bottom:8px; margin-right:10px; margin-top:10px;" src="file://nDrOoULI.png" width="350" alt="Mau-Mau Cards">
One of the most famous German card games (also popular in some other countries) is called "Mau-Mau".  It is usually played by two to four players with a 32-card-deck of French playing cards. Your task will be to simulate a Mau-Mau game given a shuffled pile of cards, knowing the sequence of cards in the pile,  the number of players, the rules of the game and the players' rules of decision.</p>
<p>The card-deck consists of <strong>four suits</strong> (clubs ♣, spades ♠, hearts <span style="color:red">♥</span>, diamonds <span style="color:red">♦</span>)  each with cards of <strong>eight ranks</strong> (seven [7], eight [8], nine [9], ten [10], jack [20], queen [3], king [4], ace [11]). Values (in square brackets) are important for decision rules  and the scoring at the end of the game. I will use a <strong>two-letter-notation</strong> for each card:  The first character is the first letter of the suit, the second one is the first letter of its rank, all upper-case, e.g.  <strong>CN</strong> (nine of clubs) or <strong>HK</strong> (king of hearts).</p>
<p style="font-size:130%; font-weight:bold">Rules of playing</p>
<p>All cards are shuffled and dealt clockwise one card at a time to each player. The number of cards for each player depends on the number of players.  Each of two players gets 7 cards, each of three players gets 6 cards and each of four players gets 5 cards.  The players take their cards, looking (only) at their own cards. After dealing cards to all players the topmost card of the pile is laid on the table faceup. This card is the first one on the <strong>discard pile</strong>.  The remaining cards are laid on the table facedown as <strong>draw pile</strong>.</p>
<p>The player, who got the first card, starts playing. If one of his cards corresponds to the suit or value of the open card (i.e. the topmost card on the discard pile), he can play this card, which means, put it faceup on top of the discard pile. Be aware, that there are some additional rules, if an "action card" is played (see below). If the player has no matching  card, he must take the upmost card of the draw pile. If that card matches, it can be put down in the same turn.  Otherwise play moves on to the next player in turn. If one player puts his last card on the discard pile, he is the winner and the game is over.</p>
<p>If the draw pile should be exhausted, the topmost card of the discard  pile is removed and the remaining discard pile is turned face down, forming the new draw pile. The removed open card is put down as new discard pile. This is done <em>immediately</em> after the last card is drawn, even if that card matches the open card and can be played in the same turn!   So the next card to draw from the draw pile will always be the bottom card of the former discard pile.  It is guaranteed that a game will not completely run out of cards. (In fact there exist a few "degenerated distributions" that lead to that state, but there is no such case among the testcases.)</p>
<p style="font-size:130%; font-weight:bold">Action cards</p>
<p><span style="color:red; font-weight:bold">Seven</span>: If a seven is played (or is the opening card on the discard pile after dealing the cards), the next player in turn has to take the two topmost cards from the draw pile as a <strong>penalty draw</strong>, even if one of his cards corresponds to the suit or is a jack.  The only card that can be played and thus will avoid the penalty draw, is another seven.  By playing another seven the move is "extended": The next player in turn now has to draw four cards – unless he has another seven and extends the move  once more by playing it. In that case the next player in turn has to draw six cards – unless he has another (the last) seven and can extend the move once again,  which results in a penalty draw of eight cards for the next player.<br> Regardless of the number of cards to draw, the "punished player" is not allowed to put a card down on the discard pile after drawing the penalty cards. The turn moves on to the next player, and the seven has lost its effect. The next player can play any matching card.</p>
<p><span style="color:red; font-weight:bold">Eight</span>: If an eight is played (or is the opening card on the discard pile after dealing the cards),   the next player in turn is skipped and the turn moves to the following player. So, if it's a two player game, the player, who played an eight, can play a second card (which again could be an eight, so he can play a third card etc.). After skipping, the eight has lost its effect. The next player can play any matching card.</p>
<p><span style="color:red; font-weight:bold">Jack</span>: The jack matches to every card except another jack or an active seven regardless of its suit. You can consider a jack to be "suitless".  Moreover a jack has the power of choosing an arbitrary suit, independed from the jack's suit.  For example you can choose "spades" playing the jack of hearts. This suit is binding for the next player(s) in turn,  as long as the jack is the topmost card on the discard pile. The next player in turn has to put down any card (except another jack), that matches the chosen suit. If the opening card is a jack, the first player may play an arbitrary card (except a jack).</p>
<p style="font-size:130%; font-weight:bold">Rules of decision</p>
<p>For the purpose of the simulation we have to lay down some rules of decision for the player being in turn. Of course, all decisions must be taken within the limits of the game's rules!</p>
<p><span style="color:red; font-weight:bold">Rule 1</span>: If you have to draw penalty cards because of an active seven and are able to extend that move by playing another seven, you do so.</p>
<p><span style="color:red; font-weight:bold">Rule 2</span>:  If you have a card other than a jack that matches the open card, you play that card.  If you have more than one of those cards, you play one with highest value.</p>
<p><span style="color:red; font-weight:bold">Rule 3</span>:  If you have no matching card other than a jack, you play a jack.</p>
<p><span style="color:red; font-weight:bold">Rule 4</span>: If the next player in turn has only one card left, you play a jack, even if you have another matching card.</p>
<p><span style="color:red; font-weight:bold">Rule 5</span>: If you play a jack, you choose the suit that is represented most among your cards as binding suit for the next player(s) in turn. If there is a tie, you choose a suit with the highest suit-rank (→ rule 6). Remember that jacks are "suitless" and thus are not taken into account here.</p>
<p><span style="color:red; font-weight:bold">Rule 6</span>: If you have more than one matching card with the same value at your disposal,  you always play the one with the highest suit-rank. The order of the suits is (from higher to lower rank): clubs, spades, hearts, diamonds.</p>
<p style="font-size:130%; font-weight:bold">End of the game</p>
<p>The game ends, when one player puts down his last card on the discard pile -  he is the winner of the game.  If this last card is an action card, that action is not executed. In particular, if this last card is a seven, the next player in turn does not have to draw the penalty cards, no matter how many that would be.</p>
<p>Finally the score for each player has to be calculated as the sum of the values of his remaining cards. The winner has a score of 0 points. If the final card played by the winner is a jack, the score for each player is doubled. The more points, the worse.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Input starts with the number t&lt;50 of testcases in a single line.  Then t lines follow, each line describing the initial state of a Mau-Mau game.  First the number of players (2, 3 or 4) followed by a single space, then 32 cards in two-letter-notation as explained above,  separated by single spaces. That sequence represents the draw pile before dealing the cards.  The first card in the sequence is the topmost card of the pile and will always be dealt to the first player.</p>
<h3>Output</h3>
<p>For each game you have to print the sequence of cards on the discard pile during the whole game in the order they were played, starting with the initial open card at the beginning of the game. You have to use the space separated two-letter-notation in a single line.<br> In a second line you have to print the final scoring. The line starts with "Score: " (without quotes) followed by the  score of the first player, second player etc., separated by single spaces (see example below).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 SS HA SN HQ CE SQ CA DT CK CQ DJ CN HN DN CS SA CJ DA HJ HS DE HT SE DK HK ST SJ HE DS CT DQ SK
3 SA SS CQ CT DA DJ ST HA SK HK DK DS DQ CE CK DE SQ DN DT SJ SE HN CJ CS HQ HJ CN HE CA HT SN HS 

<strong>Output:</strong>
CS SS SN SA CA HA HN CN CE CK CJ DA DJ HQ HS
Score: 0 45
DT CT CE DE DN DQ DA DS SS SA HA HN HK DK CK SJ SQ
Score: 18 0 47
</pre>
<div style="background-color:#f8ffc9; padding:15px;margin-top:30px">
<p style="font-weight:bold">Explanation of the first example</p>
<p>After dealing, the cards are distributed as follows.</p>
<pre style="font-weight:bold; color:green">player 1: SS SN CE CA CK DJ HN      player 2: HA HQ SQ DT CQ CN DN
discard pile: CS
draw pile:    SA CJ DA HJ HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>The order of the players' cards corresponds to the process of dealing. The discard pile grows to the right (bottom card is left), the draw pile has its topmost card on the left.<br> The open card is an action card, player 1 has to draw two penalty cards. But as he has a seven, he plays SS and extends that move. Player 2 now has to draw four penalty cards. As he has no seven, he has to draw. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: SN CE CA CK DJ HN         player 2: HA HQ SQ DT CQ CN DN SA CJ DA HJ
discard pile: CS SS
draw pile:    HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 1 is in turn, because player 2 is not allowed to play a card after drawing penalty cards. The only (non-jack) card that matches is SN, so he has to play it. Player 2 has four matching cards (SQ CN DN SA) and plays SA as this card has the heighest value of all matching cards. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: CE CA CK DJ HN            player 2: HA HQ SQ DT CQ CN DN CJ DA HJ
discard pile: CS SS SN SA
draw pile:    HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 1 is in turn. The only card that matches is CA, so he plays it. Player 2 plays his highest value matching card which is HA. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: CE CK DJ HN               player 2: HQ SQ DT CQ CN DN CJ DA HJ
discard pile: CS SS SN SA CA HA
draw pile:    HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 1 is in turn. The only card that matches is HN, so he plays it. Player 2 plays his heighest value matching card which is CN. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: CE CK DJ                  player 2: HQ SQ DT CQ DN CJ DA HJ
discard pile: CS SS SN SA CA HA HN CN
draw pile:    HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 1 is in turn. He has two matching cards and plays CE because of the higher value. CE is an action card, the next player in turn is skipped, which is player 2. So, player 1 is in turn again. He plays CK as this is his only matching card. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: DJ                        player 2: HQ SQ DT CQ DN CJ DA HJ
discard pile: CS SS SN SA CA HA HN CN CE CK
draw pile:    HS DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 2 is in turn. He has a single matching non-jack card (CQ), but as the next player in turn has only one card left, he plays a jack instead. He has two jacks at his disposal, so he chooses the one with higher suit-rank and plays CJ. The suit represented most among his cards is diamonds, so he chooses diamonds as binding color. The last card of player 1 is a jack, but that can't be played, because of the jack on the discard pile. So he has to draw one card. Player 1 is still in turn, but the drawn card does not match to the binding color, so he looses his turn. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: DJ HS                     player 2: HQ SQ DT CQ DN DA HJ
discard pile: CS SS SN SA CA HA HN CN CE CK CJ
draw pile:    DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 2 is in turn. He has three matching cards and plays DA because of the highest value. Player 1 has no matching non-jack card, so he plays his jack. As his one and only left card is of hearts, he chooses hearts as binding color. After that the cards are distributed as follows:</p>
<pre style="font-weight:bold; color:green">player 1: HS                        player 2: HQ SQ DT CQ DN HJ
discard pile: CS SS SN SA CA HA HN CN CE CK CJ DA DJ
draw pile:    DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>Player 2 is in turn. Again the next player has only one card left, so he decides to play a jack instead of another matching card. Unfortunately there is a jack on the discard pile, so he is not allowed to play a jack, and plays his only matching non-jack card HQ. Player 1 is in turn. His last card matches, so he plays it and is the winner of the game. Though his last card was an action card, player 2 does not have to draw the two penalty cards according to the rules. So, the final distribution is as follows:</p>
<pre style="font-weight:bold; color:green">player 1:                           player 2: SQ DT CQ DN HJ
discard pile: CS SS SN SA CA HA HN CN CE CK CJ DA DJ HQ HS
draw pile:    DE HT SE DK HK ST SJ HE DS CT DQ SK</pre>
<p>The scoring of player 2 is: 3+10+3+9+20 = 45</p>
</div>