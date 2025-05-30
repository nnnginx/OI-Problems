<p>A company "ACM Foods" is preparing for opening its chain shop in a certain area, but another company "ICPC
Pizza" is also planning to set up its branch shop in the same area. In general, two competitive shops gain less
incomes if they are located so close to each other. Thus, if both "ACM Foods" and "ICPC Pizza" went on
opening, they would be damaged financially. So, they had a discussion on this matter and made the following
agreement: only one of them can branch its shop in the area. It is determined by Rock-Paper-Scissors (RPS)
which to branch the shop.</p>
<p>ACM Foods is facing financial difficulties and strongly desires to open their new shop in that area. The executives
have decided to make every effort for finding out a very strong RPS player. They believes that players who win
consecutive victories must be strong players. In order to find such a player for sure, they have decided their
simple strategy.</p>
<p>In this strategy, many players play games of RPS repeatedly, but the games are only played between players with
the same number of consecutive wins. At the beginning, all the players have no wins, so any pair of players
can play a game. The games can be played by an arbitrary number of pairs simultaneously. Let us call a set of
simultaneous games as a turn. After the first turn, some players will have one win, and the other players will
remain with no wins. In the second turn, some games will be played among players with one win, and some
other games among players with no wins. For the former games, the winners will have two consecutive wins,
and the losers will lose their first wins and have no consecutive wins. For the latter games, the winners will have
one win, and the losers will remain with no wins. Therefore, after the second turn, the players will be divided
into three groups: players with two consecutive wins, players with one win, and players with no wins. Again,
in the third turn, games will be played among players with two wins, among with one win, and among with no
wins. The following turns will be conducted so forth. After a sufficient number of turns, there should be a player
with the desired number of consecutive wins.</p>
<p>The strategy looks crazy? Oh well, maybe they are confused because of their financial difficulties.
Of course, this strategy requires an enormous amount of plays. The executives asked you, as an employee of
ACM Foods, to estimate how long the strategy takes. Your task is to write a program to count the minimum
number of turns required to find a player with M consecutive wins among N players.</p>

<h3>Input</h3>
<p>The input consists of multiple test cases. Each test case consists of two integers N (2 �� N �� 20) and M (1 �� M &lt; N) in one line.</p>
<p>The input is terminated by the line containing two zeroes.</p>

<h3>Output</h3>
<p>For each test case, your program must output the case number followed by one integer which indicates the minimum number of turns required to find a person with M consecutive wins.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2 1
10 5
15 10
0 0

<b>Output:</b>
Case 1: 1
Case 2: 11
Case 3: 210
</pre>