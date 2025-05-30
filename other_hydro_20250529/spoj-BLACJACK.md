<p>You, as a great mathematician and a former member of Blackjack Team, are recently declared "unwelcome person" by managers of local casinos. Extremely bored, you reminded of your life forming a team beating casinos at blackjack worldwide, and decided to help your friends in winning blackjack games.</p>
<p>Blackjack, also known as twenty-one, is a game frequently seen in casinos, played with one deck, or several decks of 52 cards. The version your friend plays is slightly different from what we used to see in usual casinos. In this version, the game is played between a player and a dealer with a deck of n cards, namely a<sub>1</sub>, a<sub>2</sub>, ... , a<sub>n</sub>, instead of regular decks of 52 cards in standard version. The <em>i</em>-th card has the unique numeric value a<sub>i</sub>, which is important in following description of rules.</p>
<p>The game is played in several rounds as long as not less than k (k &gt;= 10) cards left in the deck. Cards are dealt from a<sub>1</sub> to a<sub>n</sub>, while each card is dealt out at most once. In each round, the player is dealt one card, then the dealer, then the player, then dealer. They now have two cards in their hand respectively. Then the player would keep on taking a hit until he busts (total value of his hand exceeds 21 points) or he feels it is enough (total value of his hand exceeds 15 points) or he has taken 3 hits already. He immediately loses the round if he busts. If he has taken 3 hits without bust, making his hand consist of 5 cards, he wins the round, ending the round right away. Then the dealer will use the exactly same strategy as the player. Of course, the dealer loses the round immediately if he busts, wins the round at once if his hand consists of 5 cards, with the same rule applying. If after taking hits neither the player nor the dealer wins or loses, sums of points (described below) in their hands will be compared, and the person with larger one will win the round. In case of tie, neither wins or loses. Of course, this ends the current round.</p>
<p>In the casino your friend plays, there is a special rule: before the game starts, the player is required to cut the deck of card exactly once. By saying cut the deck we mean to change deck of cards from</p>
<pre>a<sub>1</sub>, a<sub>2</sub>, ... , a<sub>n</sub>
</pre>
<p>to</p>
<pre>a<sub>p</sub>, a<sub>p+1</sub>, ... , a<sub>q</sub>, a<sub>1</sub>, a<sub>2</sub>, ... , a<sub>p-1</sub>, a<sub>q+1</sub>, ... , a<sub>n</sub>(1 &lt; p &lt;= q &lt; n)
</pre>
<p>With your super power (in hacking) you now know the deck of cards to play. Now you want to instruct your friend to cut the cards by telling your friend p and q in a secret manner, in order to maximize number of rounds he wins.</p>
<h3>Input</h3>
<p>There are several test cases, the number of them is about 15.</p>
<p>For each test case, the first line contains two integers, namely n (20 &lt;= n &lt;= 2000) and k (10 &lt;= k &lt;= n).</p>
<p>The following lines contain totally n characters separated by spaces or line breaks. Characters can be any of A,2,3,4,5,6,7,8,9,T,J,Q,K where A stands for numeric 1 and T,J,Q,K stands for numeric 10.</p>
<p>Input is terminated by EOF.</p>
<h3>Output</h3>
<p>For each test case, output one line "Case X: Y" where X is the test case number (starting from 1) and Y is a number indicating the desired answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
20 10
8 4 7 8 8 K 5 A Q Q A Q 6 4 J 6 9 5
3 9
40 10
3 J 7 7 2 T J 6 A 4 4 8 J T 6 A 6 2 K 9
6 5 7 J T 3 5 5 3 7 7 J 5 3 A 5 9 Q 6 7

<strong>Output:</strong> 
Case 1: 3
Case 2: 6
</pre>