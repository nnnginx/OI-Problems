<p>
	Last year there were a lot of complaints concerning the set of problems. Most 
	contestants considered our problems to be too hard to solve. One reason for 
	this is that the team members responsible for the problems are not able to 
	evaluate properly whether a particular problem is easy or hard to solve. (We 
	have created until now so many problems, that all seems quite easy.) Because we 
	want our future contests to be better we would like to be able to evaluate the 
	hardness of our problems after the contest using a history of submissions.
</p>
<p>
	There are a few statistics that we can use for evaluating the hardness of a 
	particular problem: the number of accepted solutions of the problem, the 
	average number of submissions of the problem and the average time consumed to 
	solve it (as "General rules" of the contest state "the time consumed for a 
	solved problem is the time elapsed from the beginning of the contest to the 
	submittal of the accepted run"). For the latter two statistics we consider only 
	the teams which solved this particular problem. Needless to say we ask you to 
	write a program that computes aforementioned statistics for all problems.
</p>
<h3>Task</h3>
<p>
	Write a program that:
</p>
<div align="justify">
	<ul>
		<li>
		reads a history of submissions during an ACM contest,
		</li><li>
		computes for each problem the number of accepted solutions of the problem, the 
		average number of submissions and the average time consumed to solve it,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, the first line of the input contains one integer n (1 &lt;= 
	n &lt;= 2000) being the number of submissions during the contest. Each of the 
	next n lines describes one submission and contains a submission time (measured 
	in seconds from the beginning of the contest), a team identifier, a problem 
	identifier and a result of evaluating the submission separated by single 
	spaces. The submission time is a positive integer not greater then 18000. The 
	team identifier is a non-empty string consisting of at most five small letters 
	or digits. The problem identifier is a capital letter A, B, ..., or I. The 
	result is a capital letter A (the submission is accepted) or R (the submission 
	is rejected).
</p>
<p>
	Submissions are given in nondecreasing order according to submission times and 
	there are 62 teams competing.
</p>
<p>
	Please note that if a problem is accepted all further submission of this 
	problem by the same team are possible but they should not be taken to the 
	statistics.
</p>
<h3>Output</h3>
<p>
	For each test case the output consists of nine lines. The first line 
	corresponds to problem A, the second line to problem B, and so on. Each line 
	should contain the problem identifier, the number of accepted solutions of the 
	problem, the average number of submissions done by teams that solved that 
	problem and the average time consumed to solve it separated by single spaces. 
	The latter two statistics should be printed only if there was at least one 
	accepted solution of the given problem and should be rounded to two fractional 
	digits (in particular 1.235 should be rounded to 1.24).
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
12 
10 wawu1 B R 
100 chau1 A A 
2000 uwr2 B A 
2010 wawu1 A R 
2020 wawu1 A A 
2020 wawu1 B A 
4000 wawu2 C R 
6000 chau1 A R 
7000 chau1 A A 
8000 pp1 A A 
8000 zil2 B R 
9000 zil2 B A 

<b><tt>Sample output:</tt></b>
A 3 1.33 3373.33 
B 3 1.67 4340.00 
C 0 
D 0 
E 0 
F 0 
G 0 
H 0 
I 0 
</pre>