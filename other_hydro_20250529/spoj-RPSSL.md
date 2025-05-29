<p>Daniel enjoys watching TV series. One of his favorite is "The Big Bang Theory". The main characters of this series are: Sheldon 每 genius theoretical physicist, his friend Leonard 每 talented experimental physicist, their attractive, blonde neighbor Penny, and also their friends  an aerospace engineer Howard and a particle astrophysicist Rajesh.<br> 
One time Rajesh tells Sheldon:<br>
※I'll tell you what. How about we go rock-paper-scissors?§<br>
※Ooh§, 每 Sheldon replies 每 ※I don't think so. Anecdotal evidence suggests that in the game of rock-paper-scissors, players familiar with each other will tie 75 to 80% of the time due to the limited number of outcomes. I suggest rock-paper-scissors-lizard-Spock§.<br>
※What?§<br>
※It's very simple. Scissors cuts paper. Paper covers rock. Rock crushes lizard. Lizard poisons Spock. Spock smashes scissors. Scissors decapitates lizard. Lizard eats paper. Paper disproves Spock. Spock vaporizes rock. And as it always has, rock crushes scissors§.<br>
※Okay, I think I got it§.<br>
And the friends decided to play rock-paper-scissors-lizard-Spock. And we would determine what the probability that Rajesh beats Sheldon in this game. We know the probabilities that any of the friends choose any object in the game. Also we know that they play till two wins, so the winner of the game is the person who first wins two rounds.

</p><h3>Input</h3>
<p>The first line of input contains the number t - the number of tests. Next comes the description of t tests. Each test case consists of two lines. The first line contains five integers R<sub>R</sub>, R<sub>Sc</sub>, R<sub>P</sub>, R<sub>L</sub>, R<sub>Sp</sub> 每 the probabilities that Rajesh chooses rock, scissors, paper, lizard or Spock respectively. The second line contains five integers S<sub>R</sub>, S<sub>Sc</sub>, S<sub>P</sub>, S<sub>L</sub>, S<sub>Sp</sub> 每 the probabilities that Sheldon chooses rock, scissors, paper, lizard or Spock respectively. (<b>Note:</b> the order of the objects in the input is rock, scissors, paper, lizard, Spock. The original problem is in Russian and we have scissors before paper in Russian variant of the game. Otherwise the rules are the same.)

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 500<br>
0 &lt;= R<sub>R</sub>, R<sub>Sc</sub>, R<sub>P</sub>, R<sub>L</sub>, R<sub>Sp</sub> &lt;= 100, R<sub>R</sub> + R<sub>Sc</sub> + R<sub>P</sub> + R<sub>L</sub> + R<sub>Sp</sub> = 100<br>
0 &lt;= S<sub>R</sub>, S<sub>Sc</sub>, S<sub>P</sub>, S<sub>L</sub>, S<sub>Sp</sub> &lt;= 100, S<sub>R</sub> + S<sub>Sc</sub> + S<sub>P</sub> + S<sub>L</sub> + S<sub>Sp</sub> = 100<br>

</p><h3>Output</h3>
<p>For each test case print the probability that Rajesh beats Sheldon in percent rounded to the nearest integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
10 20 30 40 0
10 10 10 10 60
20 20 20 20 20
20 20 20 20 20

<b>Output:</b>
66
50

</pre>