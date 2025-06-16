<p>Charles is the contest director for the ICPC Tumbolian regional contest. His responsibility is
ensuring the contest flows smoothly, that the contest rules are applied fairly, and, of course,
announcing the final contest ranking.

</p><p></p><p>
According to ICPC rules, a team with more solved problems ranks above a team with less
solved problems. If two teams have the same number of solved problems, the team with the
smaller total penalty ranks above the team with the larger total penalty (in case both teams
have the same number of solved problems and the same penalty, Charles considers them as
tied).

</p><p></p><p>
The <i>total penalty</i> for a team is the sum of all the problem penalties of the problems that team
has solved. The problem penalty for a problem is TP +EP ��FA, where TP is the time penalty
for that problem, EP is the contest��s error penalty and FA is the number of failed attempts
at solving the problem before submitting a correct solution.

</p><p></p><p>
The <i>time penalty</i> for a problem is the time since the start of the contest, in minutes, that the
team needed to solve the problem. The <i>error penalty</i> is a positive integer chosen by the contest
director, designed to reward teams that submit correct solutions on the first attempt.

</p><p></p><p>
Charles wants to change the error penalty from the ��standard�� value of 20 minutes to stir things
up. To study the effects of that change on the final rankings, he wants to know the range of
error penalties that <i>don��t</i> change the final standings.

</p><p></p><p>
In other words, if team A is ahead of team B in the original standings, then A should be ahead
of B in the modified standings; if A and B are tied in the original standings, they should also
be tied in the modified standings (the original standings are the ones obtained with an error
penalty of 20 minutes).

</p><p></p><p>
Charles has been very busy organizing the Tumbolian regional, so he asked you to make a
program that will compute the range for him.

</p><h3>Input</h3>
<p>The input contains several test cases. The first line of each test case contains two integers
T and P separated by a single space, indicating the number of teams and the number of
problems, respectively (2 &lt;= T &lt;= 100, 1 &lt;= P &lt;= 10). Each one of the next T lines describes
the performance of a team. A team��s performance description is a line containing P problem
descriptions separated by single spaces. Teams are not necessarily given in order of their final
standings.

</p><p></p><p>
Each problem description is a string ��A/S��, where A is an integer representing the number of
attempts that the corresponding team made at solving that problem (0 &lt;= A &lt;= 100), and S
is either ��-��, if the team did not solve that problem, or an integer indicating the number of
minutes it took for the team to submit a correct solution (1 &lt;= S &lt;= 300). Attempts made after
the first correct submission are not counted.

</p><h3>Output</h3>
<p>For each test case in the input print two positive integers separated by a single space, indicating
the smallest and largest error penalties that would not change the final ranking. If there is no
upper bound for the error penalty, print a ��*�� instead of the upper bound.

</p><h3>Example</h3>

<pre><b>Input:</b>
5 3
0/- 0/- 0/-
2/- 2/- 1/-
1/60 1/165 1/-
1/80 0/- 2/120
0/- 1/17 0/-
4 2
17/- 5/-
2/7 3/-
3/- 2/-
1/15 0/-
3 2
1/- 2/15
2/53 1/17
1/70 1/20
0 0

<b>Output:</b>
1 24
9 *
20 20
</pre>