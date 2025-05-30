<p>On Monday, the number of frosh were reduced in half.  To further reduce the number of engineers to a manageable number, the following challenge was devised for the second day.  Each of the students would have to take this challenge individually.<br><br>
Each student would be placed at a vertex of perimeter fence of Waterloo (oh yeah, some background: to keep UofT��s engineering Lady Godiva band out of Waterloo, a fence was erected surrounding the university.  The fence just happens to be an N-gon).  At some other vertex along the fence would be located a temptation so seductive that no Waterloo student could resist �C an extra-credit assignment.  The challenge of each student is to go from his starting vertex to the vertex with the prize.  There are however 3 rules:
<br><br>
a)	The student can only travel from vertex to vertex (backwards or forwards) along the polygonal fence.<br><br>
b)	The student has to make contact with exactly K vertices (the vertex he starts at doesn��t count unless he returns to it).  The K vertices need not be unique.  The final vertex has to be the one with the prize.<br><br>
c)	If the student cannot reach the prize and make contact with exactly K vertices, he fails the test and is kicked out of the university.<br><br>

Of course, no Waterloo student is satisfied with only 1 solution to any problem.  Therefore, inevitably, each student determines all ways that he/she can win.  Note that there may be no solution to the problem (the astute student has figured out that this will result in a class size of 0 �C this is entirely allowable as the variable used to quantify enrollment was incorrectly defined as a whole number instead of a natural number).<br><br>

</p><h3>Input</h3>
<p>N K (N, K &lt;= 50)<br>
A B (A = the starting vertex number, B = destination vertex number)<br>
-1 -1 terminates input<br><br>

</p><h3>Output</h3>
<p>The total number of ways of reaching the destination from the starting point by following the above rules.  The total number of ways will be less than 2<sup>63</sup> - 1.  Output 0 if there are no solution.

</p><h3>Example</h3>

<pre><b>Input:</b>
8 5
1 4
-1 -1

<b>Output:</b>
6
</pre>