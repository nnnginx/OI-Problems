<p align="justify">
 We consider only special type of tournaments. Each tournament consists of a series of matches. We have <i>n</i> competitors at the beginning of a competition and after each match the loser is moved out of the competition and the winner stays in (there are no draws).
The tournament ends when there is only one participant left - the winner.
It is a task of National Sports Federation to schedule the matches.
Members of this committee can pick the contestants for the first match. Then, after they know the result, they say which of the remaining contestants meet in the second match,
and so on until there is only one participant left. 
<br>
It is easy to see that not only skill and training decides about the win, but also
"luck" - i.e. the schedule. The members of NSF know it as well.
<br>
The committee used the training time to look carefully on the performance of each probable contestant. It is clear now, at the start of the season, that some of the results between the competitors are 100% predictable. Having this information
NSF considers if it is possible to schedule the matches in such a way that the given contestant <b> x</b> wins. That is to plan the matches for <b>x</b> only with those who will lose with him (then he wins the whole tournament of course).
If it is possible then w say that <b>the tournament can be set for x</b>.
</p>
<h3>Task</h3>
<p align="justify">
Your task is to write a program which determines 
the number of contestants of a given tournament for which it is possible to set it.
</p>
<h3>Input</h3>
<p align="justify">
t [number of tests to solve].
<br>
In the first line of each test:
n (1&lt;=n&lt;=1000) - the number of participants of the tournament. We number the participants with numbers 1,2, ... ,n. 
The following line contains a list of participants who will inevitably win with participant 1. This list begins with a number <i>m</i> (the number of contestants "better" than 1) and numbers n<sub>1</sub>,n<sub>2</sub>, ... , n<sub>m</sub> 
delimited by single spaces. <br>
Next <i>n-1</i> lines contain analogous lists for participants 2, 3, ..., n.
<br>
Remark 1. The fact that participant <b>a</b> would lose with <b>b</b> and <b>b</b>
would lose with <b>c</b> doesn't necessarily mean that <b>a</b> would lose with <b>c</b> in a direct match.
<br>
Remark 2. It is not possible that <b>a</b> is on the list of contestants better than <b>b</b> and <b>b</b> is on the list of <b>a</b> at the same time.
</p>
<h3>Output</h3>
<p align="justify">
For each test your program should output a single integer - the number of participants, for which it is possible to set the tournament.
</p>
<h3>Example</h3>
<pre>Input:
1
3
2 3 2
1 3
0
Output:
1
</pre>