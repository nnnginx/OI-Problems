<p>After eating dinner at a restaurant with some friends, you determine
how much money each person owes. Each of you has some cash and some
change, but very few of you have exact change. Can you make change
for each other so that each person ends up paying the exact right
amount?

</p><h3>Input</h3>
<p>The input file will contain multiple cases. The first line of each
case is N, the number of people at the table. This is followed
by N lines, one for each i ¡Ê [1,N], containing

<br>

</p><center><table width="100%" border="0">
<tbody><tr>
<td>x<sub>i</sub></td> <td>c<sub>i,1</sub></td> <td>c<sub>i,5</sub></td> <td>c<sub>i,10</sub></td> <td>c<sub>i,25</sub></td> <td>c<sub>i,100</sub></td> <td>c<sub>i,500</sub></td> <td>c<sub>i,1000</sub></td> <td>c<sub>i,2000</sub></td> <td>c<sub>i,5000</sub></td> <td>c<sub>i,10000</sub></td>
</tr>
</tbody></table></center>

<p>where x<sub>i</sub> is the amount in cents that person i owes and c<sub>i,v</sub>
is the number of coins or bills worth v cents that person i
starts out with. For example, person 1 has c<sub>1,1</sub> pennies, c<sub>1,5</sub>
nickels, etc.

Each case is followed immediately by the next case. The end of the
input is indicated by a line containing only a zero.

You may assume that no person owes more money than they have (i.e.
x<sub>i</sub> ¡Ü ¦²<sub>j</sub> j*c<sub>i,j</sub>) and that the total amount of money in cents that
everyone starts with fits in a signed 32-bit integer. You may also
assume that N ¡Ü 100000.

</p><h3>Output</h3>
<p>For each case, output the case number, in the format "Case #:" (where # is the case number, starting at 1), followed by
a space, followed by "YES" if all of the money can
be rearranged so that each person ends up paying the correct amount
and "NO" if not.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
10 0 0 1 0 0 0 0 0 0 0
2
0 0 0 0 0 2 0 0 0 0 0
500 0 0 0 0 0 1 0 0 0 0
1
100 4 0 2 3 0 1 0 0 0 0
0

<b>Output:</b>
Case 1: YES
Case 2: YES
Case 3: NO
</pre>