<p>
Sheikh Abdul really loves football. So you better don't ask how much
money he has spent to make famous teams join the annual tournament.
Of course, having spent so much money, he would like to see certain
teams play each other. He worked out a complete list of games
he would like to see. Now it is your task to distribute these games into rounds
according to following rules:<br>
</p>
<ul>
  <li>In each round, each remaining team plays at most one game</li>
  <li>If there is an even number of remaining teams, every team plays
exactly one game</li>
  <li>If there is an odd number of remaining teams, there is exactly
one team which plays no game
(it advances with a wildcard to the next round)</li>
  <li>The winner of each game advances to the next round, the loser is
eliminated from the tournament</li>
  <li>If there is only one team left, this team is declared the winner
of the tournament</li>
</ul>
<p>
As can be proved by induction, in such a tournament with <i>n</i>
teams,
there are exactly <i>n - 1</i> games required until a winner is
determined. <br>
Obviously, after round 1, teams may already have been eliminated which should take
part in another game. To prevent this, for each game you also have to
tell which team should win.</p>
<h3>Input Specification</h3>
<p>The input file contains several test cases.<br>
Each test case starts with an integer <i>n</i> (<i>2 �� n ��
1000</i>),
the number of teams participating in the tournament.
The following <i>n</i> lines contain the names of the teams
participating in the tournament. You can assume that each team name
consists of up to <i>25</i> letters of the English alphabet
('a' to 'z' or 'A' to 'Z').<br>
Then follow <i>n - 1</i> lines, describing the games the sheikh
would like to see (in any order). Each line consists of the two names of the teams
which take part in that game. You can assume that it is always
possible to find a tournament schedule consisting of the given games.<br>
The last test case is followed by a zero.
</p>
<h3>Output Specification</h3>
<p>For each test case, write the game schedule, distributed in rounds.<br>
For each round, first write "Round #X" (where X is the round number)
in a line by itself. Then write the games scheduled in this round
in the form: "A defeats B", where A is the name of the advancing team
and B is the name of the team being eliminated. You may write the games
of a round in any order. If a wildcard is needed
for the round, write "A advances with wildcard" after the last game of the round, where A is the name of
the team which gets the wildcard. After the last round, write the winner in the format shown below.
Print a blank line after each test
case.<br>
</p>
<h3>Sample Input</h3>
<pre>3
A
B
C
A B
B C
5
A
B
C
D
E
A B
C D
A E
C E
0
</pre>
<h3>Sample Output</h3>
<pre>Round #1
B defeats A
C advances with wildcard
Round #2
C defeats B
Winner: C

Round #1
A defeats B
C defeats D
E advances with wildcard
Round #2
E defeats A
C advances with wildcard
Round #3
E defeats C
Winner: E

</pre>
<hr>
<i>Note that there is always more than one possible game schedule;
you may print any of them.</i>