<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MAJSTOR/en/">English</a></td> 
<td width="50%"><a href="/problems/MAJSTOR/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Rock-paper-scissors is a popular two-player game. In the game, each of the players uses their hand to
show one of three symbols: rock, paper or scissors. If both players show the same symbol, the game is
a tie. Otherwise, scissors beat paper, paper beats rock and rock beats scissors.</p>
<p>Sven has been studying the psychological intricacies of the game for years and has become a real master
at the game, his friends not standing a chance against him in one-on-one games.</p>
<p>With the world championships around the corner, Sven is practicing his skills playing simultaneous
games with N of his friends. One such game consists of R rounds. In each round, Sven and each of his
friends show one of the three symbols.</p>
<p>When calculating the score, in each round, Sven's symbol is independently compared to each of his
friends' symbols. Sven scores two points for every win and one point for every tie. Sven does not get
points for losing.</p>
<p>Write a program that calculates Sven's total score, and also his largest possible score had he known in
advance all the symbols his friends would show.</p>

<h3>Input</h3>
<p>The first line contains the integer R (1 ¡Ü R ¡Ü 50), the number of rounds played.</p>
<p>The second line contains a string of R letters 'S', 'P' or 'R'. The string represents symbols that Sven
showed in each round. 'S' is for scissors, 'P' for paper, 'R' for rock.</p>
<p>The third line contains the integer N (1 ¡Ü N ¡Ü 50), the number of friends.</p>
<p>Each of the following N lines contains a string of R letters 'S', 'P' or 'R'. These are the symbols shown
by each of the N friends in each of the R rounds.</p>

<h3>Output</h3>
<p>Output Sven's actual score on the first line.</p>
<p>Output his largest possible score on the second line, assuming his friends didn't change their symbols.</p>
<h3>Example</h3>

<pre>Input
5
SSPPR
1
SSPPR

Output
5
10


Input
5
SSPPR
2
PPRRS
RRSSP

Output
10
15


Input
4
SPRS
4
RPRP
SRRR
SSPR
PSPS

Output
12
21
</pre>