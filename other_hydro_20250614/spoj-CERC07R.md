<p>Roshambo - this simple game is known all around the world. In German, it is called "Schnick,
Schnack, Schnuck", in Japanese "Janken", in Spanish "Cachipún",in Polish "Papier, kamień, nożyce".
The Czechs call it "Kámen, nůžky, papír".

</p><p>Whatever is the name of the game, its principles remain the same. Two players simultaneously
form their hand into one of three possible shapes (symbols): Rock (closed fist), Paper (open
hand), or Scissors (two fingers extended). If both of them show the same symbol, it is a tie
and no points are given. Otherwise, one of the symbols wins: Rock blunts Scissors, Scissors cut
Paper, and Paper covers Rock.

</p><p>Czech Technical University students also know the game very well and use it to resolve small
disputes. Imagine, for example, two students living together in one room. Yesterday evening,
there was a small celebration, and in the morning, no one wants to go to the lectures. They
agreed that one person would be enough to take notices for both, but who will be the poor one.
Roshambo is a very effective way to decide.

</p><p>Did you know there are even the World Series of Roshambo. Our organizing team would like
to host the World Championships in 2009. Your task is to help us in developing a Roshambo
scoring system and write a program that evaluates one game between two players.

</p><p>Since the participants will come from different countries, the system must accept input in various
languages. The following table shows names of three Roshambo symbols. Note that in some
languages, there may be two different words for the same symbol.

</p><p>
</p><table border="1">
  <tbody><tr><td><b>Language</b></td>
      <td><b>Code</b></td>
      <td><b>Rock</b></td>
      <td><b>Scissors</b></td>
      <td><b>Paper</b></td>
  </tr>
  <tr><td>Czech<br>English<br>French<br>German<br>Hungarian<br>Italian<br>Japanese<br>Polish<br>Spanish</td>
  <td>cs<br>en<br>fr<br>de<br>hu<br>it<br>jp<br>pl<br>es</td>
  <td>Kamen<br>Rock<br>Pierre<br>Stein<br>Ko | Koe<br>Sasso | Roccia<br>Guu<br>Kamien<br>Piedra</td>
  <td>Nuzky<br>Scissors<br>Ciseaux<br>Schere<br>Ollo | Olloo<br>Forbice<br>Choki<br>Nozyce<br>Tijera</td>
  <td>Papir<br>Paper<br>Feuille<br>Papier<br>Papir<br>Carta | Rete<br>Paa<br>Papier<br>Papel</td>
 </tr>
</tbody></table>

<h3>Input</h3>
<p>The input contains several games. Each game starts with two lines describing players. Each of
these two lines contains two lowercase letters specifying the language used by the player (see the
language code in the table above), one space, and a player name. The name will consist from
at most twenty upper- or lower-case letters.

</p><p>After the players description, there are at most 100 lines containing individual rounds. Each
round is described by two words separated with one space. The words name the symbol shown
by the first and second player, respectively. All symbols are named in the mother tongue of the
concerned player. All allowed words are shown in the table above, the first letter will be always
in uppercase, all other letters in lowercase.

</p><p>The last round is followed by a line containing one single dash character ("-") and then the next game begins. The only exception is the last game in the input, which is terminated by a dot
(".") instead of the dash.


</p><h3>Output</h3>
<p>For each game, print five lines of output. The first line should contain the string "Game #G:",
where G is the number of the game, starting with one.

</p><p>The second line will contain the first player name followed by a colon (":"), one space and the
number of rounds won by that player. The number should be followed by one space and the
word "points". Use the singular form "point" if (and only if) the number of points of the
player equals one.

</p><p>The third line has the same format and shows the second player's name and points.

</p><p>The fourth line displays the outcome of the game. It must contain the word "WINNER" followed
by a colon, space and the name of the player who gained more points. If both players have the
same number of points, the fourth line will contain words "TIED GAME" instead.

</p><p>The fifth line is left empty to visually separate individual games.

</p><h3>Example</h3>
<pre><b>Input</b>
cs Pepik
en Johnny
Nuzky Scissors
Papir Rock
Papir Scissors
-
de Gertruda
cs Lenka
Stein Papir
Schere Kamen
.

<b>Output</b>
Game #1:
Pepik: 1 point
Johnny: 1 point
TIED GAME

Game #2:
Gertruda: 0 points
Lenka: 2 points
WINNER: Lenka

</pre>