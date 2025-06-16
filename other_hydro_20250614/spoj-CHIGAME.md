<p style="margin-bottom: 0in" align="JUSTIFY"><span lang="en-US">Little Mark went to China and learned an ancient chinese game dating from the 3</span><sup><span lang="en-US">rd</span></sup><span lang="en-US"> century. In this game every player chooses two numbers A, B (all pairs of numbers B must be coprime). The players gather around in a circle. Initially each player puts A beans in front of the player on his left. At this point each player writes down on their notebook the number of beans he has in front of him. Now the game starts by rounds. On every round each player will place B beans in front of the player at his right. Then each player writes down on their notebook the number of beans in front of them. The rounds keep going until there is a number C that all players have written on their notebook. The winner is the player with more numbers written before C.</span></p>
<p style="margin-bottom: 0in" lang="en-US" align="JUSTIFY">For example, lets suppose there are three players, Mark, George and Mike. They choose the numbers 15 5, 17 8 and 16 7 respectively. Initially Mark would put 15 beans in front of Mike, George would put 11 beans in front of Mark and Mike would but 16 beans in front of George. Then everybody writes down the  number in front of them (17,16 and 15). Now on each round Mark will put 5 beans in front of George, George will put 8 beans in front of Mike, and Mike will put 7 beans in front of Mark. The following table summarizes the numbers written on each person��s notebook:</p>
<p style="margin-bottom: 0in" lang="en-US" align="JUSTIFY">&nbsp;</p>
<table border="0">
<tbody>
<tr>
<td>Mark</td>
<td>George</td>
<td>Mike</td>
</tr>
<tr>
<td>17</td>
<td>16</td>
<td>15</td>
</tr>
<tr>
<td>24</td>
<td>21</td>
<td>23</td>
</tr>
<tr>
<td>31</td>
<td>26</td>
<td>31</td>
</tr>
<tr>
<td>38</td>
<td>31</td>
<td>39</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in" lang="en-US" align="JUSTIFY">The last row of the table is the last round of the game, since the number 31 has already been written down by each player. So now the winner is George, since he has 3 numbers written before the 31.</p>
<p style="margin-bottom: 0in" lang="en-US" align="JUSTIFY">Your task is to print the amount of numbers that the winner wrote before the common number C showed up. Since the game can get quite boring, in all the games the winner will have less than 2^31 numbers written on his notebook.</p>
<h3>Input</h3>
<p style="margin-bottom: 0in" lang="en-US" align="JUSTIFY">The input will begin with the number N of players (2&lt;=N&lt;=10). Following, there will be N lines, each containing a pair of numbers Ai, Bi (0&lt;=A&lt;=10^6, 2&lt;=B&lt;=10^2) indicating the numbers A and B for player i.</p>
<p style="margin-bottom: 0in" lang="en-US">The end of the input will be a case with N=0</p>
<h3>Output</h3>
<p style="margin-bottom: 0in" lang="en-US">For each test case on the input you must print a line containing the amount of lines that the winner wrote before the common number C.</p>
<h3>Example</h3>
<pre><b><u>Input:</u></b>
3
15 5
17 8
16 7
2
1 2
1 3
0

<b><u>Output:</u></b>
3
0<br></pre>