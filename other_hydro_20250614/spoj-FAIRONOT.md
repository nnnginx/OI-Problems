<p>It is not an easy job to be a coach of a football team. Especially if you do not coach great teams like Ajax, Inter, Dynamo (ok, fill in the name of your dream team), but only a mediocre one like FC Dead Horse, playing in the second league. The season is almost over, only a few matches are left to play. All of sudden the team manager comes to you and tells you bad news: the main sponsor of your club is not happy with your results and decided to stop sponsoring your team, which probably means the end of your club. The sponsor's decision is final and there is no way to change it unless... unless your team miraculously wins the league.

</p><p>The manager left you in deep thought. If you increase the number of practices and offer players a generous bonus for each match, you may be able to win all the remaining matches. Is that enough? You also have to make sure that teams with many points lose against teams with few points so that in the end, your team will have more points than any other team. You know some of the referees and can bribe them to manipulate the result of each match. But first you need to figure out how to manipulate the results and whether it is possible at all. </p>

<h3>Problem Description</h3>
<p>There are N teams numbered 1 through N, your team has the number N. The current number of points of each team and the list of remaining matches are given. Your task is to find out whether it is possible to manipulate each remaining match so that the team N will finish with strictly more points than any other team. In every match, the winning team gets 2 points, the losing team gets 0. If the match ends with a draw, both teams get 1 point. </p>

<h3>Input file specification</h3>
<p>The input file consists of several blocks. Each block has the following form: The first line contains two numbers N(1&lt;= N &lt;=100) and M(0&lt;= M &lt;=1000). The next line contains N numbers separated by spaces giving the current number of points of teams 1, 2, ..., N respectively. The following M lines describe the remaining matches. Each line corresponds to one match and contains two numbers a and b (a not equal to b) identifying the teams that will play in the given match. The last block is followed by a "-1"(without quotes) on a separate line.</p>

<h3>Output file specification</h3>
<p>For each block in the input file, output YES if you can manipulate the remaining matches so that the team N would win the league, or NO otherwise. </p>

<h3>Example</h3>
<pre><b>Input file:</b>
5 8
2 1 0 0 1
1 2
3 4
2 3
4 5
3 1
2 4
1 4
3 5
5 4
4 4 1 0 3
1 3
2 3
3 4
4 5
-1

<b>Output file:</b>
YES
NO
</pre>