<p> As you may know, planets of Alpha Centauri (if they indeed do exist) 
would provide excellent conditions for intelligent life forms. <br><br>

It is indeed true that there is a small Earthlike planet near Alpha 
Centauri, inhabited by a population of no particular significance. 
These humanlike creatures have much in common with us. Living in 
similar comunities and having similar body structure and behavioral 
patterns, they unsurprisingly appreciate (approximately) the same 
time-killing activities as we do. One of these, the second most 
popular after Alpha Centauri Croquet, is the Alpha Centauri Tennis. <br><br>

Although its rules differ from Earth Tennis, the two player 
version of Alpha Centauri Tennis resembles it in many ways. 
Same as Earth Tennis, it is played on a rectangular court 
divided into two parts by a net. Two players, standing on 
opposite sides of it, use a stringed racket to hit a ball 
back and forth to each other. There are certain rules how 
to hit the ball. The player who forces his opponent to 
violate one of these rules wins the current ball. The aim
 of both players is to win enough balls to win a game, enough
 games to win a set and enough sets to win the whole match. 
In the N player version of the Alpha Centauri Tennis a ball 
can be won by any one of the N players. Although technical 
details of this can be difficult to imagine, Alpha Centaurians 
are extremely inventive. <br><br>

In the general N-player version, players serve in turns, 
following order determined before the match. Moreover, 
they shift when starting individual games and sets. For 
example, the players are A, B and C. They are ordered 
alphabetically. Player A serves the first ball of the 
first game. When the ball is won by one of the players, 
its B's turn to serve. After the game is won by one of
the players, player B starts the second game. Finally,
when the first set is won by someone, player B starts 
the second set. This repeats, always shifted by one player, 
until the match ends. <br><br>

For three players the serving order looks as follows: <br>
Set 1: <br>
Game 1: A,B,C,A,B,C... <br>
Game 2: B,C,A,.... <br>
Game 3: C,A,B,.... <br>
Game 4: A,B,C,.... <br>
... <br>
Set 2: <br>
Game 1: B,C,A,B,.... <br>
Game 2: C,A,B,.... <br>
Game 3: A,B,C,A,... <br>
... <br>

There are exact rules for counting the number of 
balls/games/sets won by a player. <br><br>

<b>RULES FOR WINNING A GAME</b><br>
The state of a game can be described by assigning a non-negative 
number of points to each of the players. At the beginning of 
a game, the score of each player is zero. <br><br>

Note: In Earth terminology, 0 points is called "love", 1 point 
is a "fifteen", 2 points is a "thirty", 3 points is a "forty" 
and 4 points is an "advantage". Be glad that you don't have to 
learn the Centaurian terminology :) <br><br>

When a player P just won a ball, the new score is determined 
by using the first rule from the list that applies to the 
situation. <br><br>

If P currently has 3 points and no other player has more than 
2 points, P wins the current game. <br>
If P currently has 4 points, he wins the game. <br>
If any other player currently has 4 points, that player 
loses one point. P gains a point. <br><br>

<b>RULES FOR WINNING A SET</b><br>
The set is won by the first player that at the same time: <br><br>

won at least 6 games in this set <br>
won at least 2 games more than any other player <br><br>

<b>RULES FOR WINNING A MATCH</b><br>
The winner is the first player to win at least three sets. 
A set in which no other player won a game counts as two won sets. <br><br>

<b>Problem specification</b><br>
An observer from the Intergalactic Tennis Federation was 
watching a tournament in Alpha Centauri Tennis. Being unable
 to understand Alpha Centaurian language, he only managed 
to write down the winner of each ball. Now, for each match, 
knowing the sequence in which the players were winning the 
balls, he would like to somehow determine its winner. <br>
<br>
</p>

<h3>Input</h3>
<p>
t - the number of test cases [t &lt;= 150]
than t test cases follows, each corresponding to 
one match. Each line contains the number of players N [N &lt;= 10] 
and a string S consisting of uppercase letters [2 &lt;= S &lt;= 50000]. 
The players are represented by the first N letters of the English 
alphabet. If the i-th letter of S is X, it means the player X 
won the i-th ball from the beggining of the match. You may assume 
that the match transcripts are correct and complete. <br>
<br>
The order in which the players serve is the same as the order of 
their letters in the English alphabet. <br>
</p>

<h3>Output</h3>
<p>For each line, output a single character, being the letter of 
the player who won the corresponding match. 
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
3 BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBB 

<b>Output:</b>
B
</pre>
<p>
(B has won two sets, each of them by winning 6 games, while A and C 
won none. Thus each of these sets counts as two and B has won the match.) </p>