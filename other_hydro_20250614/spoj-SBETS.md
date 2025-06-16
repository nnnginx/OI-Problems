<p>The teams have finished the group stage of the FIFA World Cup and the teams that are in the round of the last sixteen are known. My boss has all of the games analyzed and bets on the whole rest of the tournament by writing the outcome of each match on a single sheet of paper. It was my job to bring his bets to the next betting office and set <em>1000</em> dollar.  Being nervous with so much cash in my pockets I fell over (I am a bit clumsy) and the bets got shuffled. So I don't know if a bet corresponds to the final match or the semi-final or something else.</p>
<p>I do not want to disappoint my boss, so I decided to place only one bet on the winner of the tournament. Everything I know is that in each round the teams that win (a team wins if it shoots more goals than the opposing team) are in the next round, the other teams are eliminated from the tournament. This is not true for the semi-finals where the losers also play for the third place. So we have in total <em>16</em> matches.</p>
<p>Can you please tell me which team will win the World Cup based on the bets of my boss?</p>
<h3>Input</h3>
<p>The first line of the input is the number of test cases <em>c</em> (<em>1 ¡Ü c ¡Ü 100</em>). Each test case consists of <em>16</em> lines describing the matches in random order. A match description looks as follows: <em>t<sub>1</sub></em> <em>t<sub>2</sub></em> <em>g<sub>1</sub></em> <em>g<sub>2</sub></em>. <em>t<sub>1</sub></em> and <em>t<sub>2</sub></em> are the names of teams (abbreviated as exactly three uppercase letters), <em>g<sub>1</sub></em> and <em>g<sub>2</sub></em> (<em>0 ¡Ü g<sub>1</sub>, g<sub>2</sub> ¡Ü 10</em>; <em>g<sub>1</sub> ¡Ù g<sub>2</sub></em>) are the goals of the two teams.</p>
<h3>Output</h3>
<p>For each test case, print one line containing the team that will win the FIFA World Cup (based on the analysis of my boss which is always correct!).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
ITA URU 2 0
ITA IRE 1 0
ITA ARG 3 4
YUG ARG 2 3
GER CZE 1 0
ENG GER 3 4
ITA ENG 2 1
CAM COL 2 1
ENG CAM 3 2
ENG BEL 1 0
GER ARG 1 0
CZE CRC 4 1
NET GER 1 2
BRZ ARG 0 1
SPA YUG 1 2
ROM IRE 4 5

<strong>Output:</strong>
GER
</pre>