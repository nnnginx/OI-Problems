<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/IZBORI/en/">English</a></td> 
<td width="50%"><a href="/problems/IZBORI/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>It is election time. V voters attend the election, each casting their vote for one of N political parties. M
officials will be elected into the parliament.</p>
<p>The conversion from votes to parliament seats is done using the D'Hondt method with a 5% threshold.
More precisely, suppose that the parties are numbered 1 through N and that they receive V1, V2, ..., VN
votes. Parliament seats are allocated as follows:</p>
<ul>
<p>1. All parties that receive strictly less than 5% of V votes are erased from the list of parties.</p>
<p>2. The parliament is initially empty i.e. every party has zero seats allocated.</p>
<p>3. For each party P, the quotient QP=VP/(SP+1) is calculated, where VP is the total number of
votes received by party P, and SP is the number of seats already allocated to party P.</p>
<p>4. The party with the largest quotient QP is allocated one seat. If multiple parties have the same
largest quotient, the lower numbered party wins the seat.</p>
<p>5. Repeat steps 3 and 4 until the parliament is full.
The votes are being counted and only part of the V votes has been tallied. It is known how many votes
each party has received so far.</p>
</ul>
<p>Write a program that calculates for each party, among all possible outcomes of the election after all V
votes are counted, the largest and smallest number of seats the party wins.</p>

<h3>Input</h3>
<p>The first line contains the integers V, N and M (1 ¡Ü V ¡Ü 10,000,000, 1 ¡Ü N ¡Ü 100, 1 ¡Ü M ¡Ü 200), the
numbers of votes, parties and seats in the parliament.</p>
<p>The second line contains N integers ¨C how many votes (of those that have been counted) each party
got. The sum of these numbers will be at most V.</p>

<h3>Output</h3>
<p>On the first line output N integers separated by spaces ¨C the largest number of seats each party can
win.</p>
<p>On the second line output N integers separated by spaces ¨C the smallest number of seats each party can
win.</p>

<h3>Example</h3>

<pre><b>Input:</b>
20 4 5
4 3 6 1

<b>Output:</b>
3 3 3 2
1 0 1 0


<b>Input:</b>
100 3 5
30 20 10

<b>Output:</b>
4 3 3
1 1 0

</pre>

<p>In the first example, 14 votes have been tallied and 6 are yet to be counted. To illustrate one possible
outcome, suppose that the first party receives 2 of those 6 votes, the second none, the third 1 vote and
the fourth 3 votes. The parties' totals are 6, 3, 7 and 4 votes. All parties exceeded the 5% threshold.
Seats are allocated as follows:</p>
<ul>
<p>1. The quotients are initially 6/1, 3/1, 7/1 and 4/1; the largest is 7/1 so party 3 wins a seat.</p>
<p>2. The quotients are 6/1, 3/1, 7/2 and 4/1; the largest is 6/1 so party 1 wins a seat.</p>
<p>3. The quotients are 6/2, 3/1, 7/2 and 4/1; the largest is 4/1 so party 4 wins a seat.</p>
<p>4. The quotients are 6/2, 3/1, 7/2 and 4/2; the largest is 7/2 so party 3 wins a seat.</p>
<p>5. The quotients are 6/2, 3/1, 7/3 and 4/2; parties 1 and 2 are tied with quotients 6/2 and 3/1,
but party 1 is lower numbered so it wins the last seat.</p>
</ul>
<p>In this outcome, the numbers of seats won by the parties are 2, 0, 2 and 1. Since it is possible for the
second party not to win any seats, the second number on the second line of output is zero.</p>