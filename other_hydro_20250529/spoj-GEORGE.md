<p>Last week Mister George visited Croatia. Since Mister George is a very important person, while he was in a street, the police <b>disallowed entry</b> to that street, but vehicles that entered the street before Mister George could continue driving.</p>
<p>While Mister George was visiting, Luka drove his truck around town. But because of some of the streets being closed off, he couldn't make his delivery in time and almost lost his job. Although it is late now, he is wondering how he could have planned his delivery better i.e. what would have been the least time needed to make his delivery while Mister George was visiting. He knows the route mister George took.</p>
<p>The city is modeled with intersections and two-way streets connecting them. For each street, Luka knows how much time he needs to traverse it (mister George needs he same amount of time).</p>
<p>For example, if Mister George starts traversing a street during minute 10 and needs 5 minutes to exit it, this street will be blocked during minutes 10, 11, 12, 13 and 14. Luka can enter the street during minutes 9 and earlier, or 15 and later.</p>
<p>Write a program that calculates the least amount of time Luka needs to make his delivery, if he starts driving K minutes after the arrival of Mister George.</p>


<h3>Input</h3>
<p>The first line contains two integers N and M (2 &lt;= N &lt;= 1000, 2 &lt;= M &lt;= 10 000), the number of intersections and the number of streets. The intersections are numbered 1 to N.
The second line contains four integers A, B, K and G (1 &lt;= A, B &lt;= N, 0 &lt;= K &lt;= 1000, 0 &lt;= G &lt;= 1000).
These are, in order:
</p><ul>
<li>The intersection where Luka starts;</li>
<li>The intersection Luka must get to;</li>
<li>The difference in starting times between mister George and Luka (Luka starts at intersection A exactly K minutes after mister George starts his route);</li>
<li>The number of intersections on Mister George's route.</li>
</ul>
The third line contains G integers, the labels of intersections mister George will visit. Every pair of adjacent integers denotes a street he will traverse. That street will exist and Mister George will traverse every street at most once.
Each of the following M lines contains three integers A, B and L, meaning that there is a street between intersection A and B, and it takes L minutes to traverse. L will be between 1 and 1000.<p></p>

<h3>Output</h3>
<p>Output the least amount of time (in minutes) Luka needs to make his delivery.</p>

<h3>Example</h3>

<pre><b>Input:</b>
6 5
1 6 20 4
5 3 2 4
1 2 2
2 3 8
2 4 3
3 6 10
3 5 15

<b>Output:</b>
21
</pre>

<hr align="center" width="50%">

<pre><b>Input:</b>
8 9
1 5 5 5
1 2 3 4 5
1 2 8
2 7 4
2 3 10
6 7 40
3 6 5
6 8 3
4 8 4
4 5 5
3 4 23

<b>Output:</b>
40
</pre>

<hr align="center">
<a href="http://www.hsin.hr/coci/">Croatian Open Competition in Informatics (COCI) - 2007/2008 Contest #6</a>