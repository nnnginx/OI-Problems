<p>This year, Egypt has been going through an extremely challenging stage. The parliamentary elections are about to take place according to a newly introduced election laws. The seats of the parliament are going to be divided in a party-list proportional representation. This type of elections allows voters to vote for a party (not for individual candidates). Each party wins a number of seats which depends on the number of votes they received.</p>
<p>You are the president of the ACM party in your electoral district (Association of Corrupt Murderers) and you want your party to win as much seats as possible in the coming elections. You know exactly how many people will vote for every party (including yours), thanks to your amazing prediction abilities.</p>
<p>There are two proposed voting systems (explained later) and it is not yet decided which of them is going to be used. You can use your connections trying to influence the decision of which voting system is put to use. Assuming your prediction is completely correct, the problem is to find the voting system that will let your party win more seats.</p>
<p><strong>Voting System 1: D'Hondt method</strong></p>
<p>This system is used in many countries, including Turkey, Japan and Spain. Let's say there are P parties and S seats. This method creates a grid of numbers, with P rows and S columns, where the entry in the i-th row and j-th column is the number of votes won by the i-th party divided by the number j. The first seat is given to the party that has the entry with the highest value. The second seat is given to the party that has the entry with the second highest value, and so on. If two or more entries have the same value, then the seat is given to the party that occurs first in the input file (for the simplicity of this problem).</p>
<p>&nbsp;</p>
<p><strong>For example</strong>: if 5 seats are to be allocated, divide each party's total votes by 1, then by 2, 3, 4 and 5. An example is given in the table below. The 5 highest five entries are highlighted in bold, ranging from 70.0 down to 30.0. The tie between party B and party D is resolved by giving the seat to B as it occurs first in the input. For each cell in bold, the corresponding party gets a seat.</p>
<table style="width: 486px;" border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="54" valign="top">
<p align="center">Party</p>
</td>
<td width="120" valign="top">
<p align="center">Number of   received votes (V)</p>
</td>
<td width="42" valign="top">
<p align="center">V/1</p>
</td>
<td width="42" valign="top">
<p align="center">V/2</p>
</td>
<td width="48" valign="top">
<p align="center">V/3</p>
</td>
<td width="54" valign="top">
<p align="center">V/4</p>
</td>
<td width="48" valign="top">
<p align="center">V/5</p>
</td>
<td width="78" valign="top">
<p align="center">Seats won</p>
</td>
</tr>
<tr>
<td width="54" valign="top">
<p align="center">A</p>
</td>
<td width="120" valign="top">
<p align="center">70</p>
</td>
<td width="42" valign="top">
<p align="center"><strong>70</strong></p>
</td>
<td width="42" valign="top">
<p align="center"><strong>35</strong></p>
</td>
<td width="48" valign="top">
<p align="center">23.3</p>
</td>
<td width="54" valign="top">
<p align="center">17.5</p>
</td>
<td width="48" valign="top">
<p align="center">14</p>
</td>
<td width="78" valign="top">
<p align="center">2</p>
</td>
</tr>
<tr>
<td width="54" valign="top">
<p align="center">B</p>
</td>
<td width="120" valign="top">
<p align="center">60</p>
</td>
<td width="42" valign="top">
<p align="center"><strong>60</strong></p>
</td>
<td width="42" valign="top">
<p align="center"><strong>30</strong></p>
</td>
<td width="48" valign="top">
<p align="center">20</p>
</td>
<td width="54" valign="top">
<p align="center">15</p>
</td>
<td width="48" valign="top">
<p align="center">12</p>
</td>
<td width="78" valign="top">
<p align="center">2</p>
</td>
</tr>
<tr>
<td width="54" valign="top">
<p align="center">C</p>
</td>
<td width="120" valign="top">
<p align="center">50</p>
</td>
<td width="42" valign="top">
<p align="center"><strong>50</strong></p>
</td>
<td width="42" valign="top">
<p align="center">25</p>
</td>
<td width="48" valign="top">
<p align="center">16.7</p>
</td>
<td width="54" valign="top">
<p align="center">12.5</p>
</td>
<td width="48" valign="top">
<p align="center">10</p>
</td>
<td width="78" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="54" valign="top">
<p align="center">D</p>
</td>
<td width="120" valign="top">
<p align="center">30</p>
</td>
<td width="42" valign="top">
<p align="center">30</p>
</td>
<td width="42" valign="top">
<p align="center">15</p>
</td>
<td width="48" valign="top">
<p align="center">10</p>
</td>
<td width="54" valign="top">
<p align="center">7.5</p>
</td>
<td width="48" valign="top">
<p align="center">6</p>
</td>
<td width="78" valign="top">
<p align="center">0</p>
</td>
</tr>
</tbody>
</table>
<p><strong>&nbsp;</strong></p>
<p><strong>Voting System 2: Sainte-Laguë method</strong></p>
<p>This system is used in fewer countries, including Norway, Sweden and Germany. This method favors smaller parties more than D'Hondt method. After the votes to each party has been counted, the parliament seats are given in an iterative way, one by one to the party that has the highest quotient. The quotient of a party is calculated by this formula:<strong> quot = V / (2s+1)</strong></p>
<p>Where:</p>
<p><strong>V:</strong> is the total number of votes that party received, and</p>
<p><strong>s:</strong> is the number of seats that party has been allocated so far, initially 0 for all parties.</p>
<p>&nbsp;</p>
<p>For simplicity, if two or more parties are tied because they have the same quotients, the party that occurs first in the input file is given the&nbsp; next seat allocated. The quotients are recalculated after each seat has been given and this process is repeated until all seats have been allocated.</p>
<p>Example: using the same example from before, in the table below:</p>
<table style="width: 570px;" border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="58" valign="top">
<p align="center">Party</p>
</td>
<td width="116" valign="top">
<p align="center">Number of   received votes (V)</p>
</td>
<td width="66" valign="top">
<p align="center"><em>quot</em> in round 1</p>
</td>
<td width="72" valign="top">
<p align="center"><em>quot</em> in round 2</p>
</td>
<td width="60" valign="top">
<p align="center"><em>quot</em> in round 3</p>
</td>
<td width="60" valign="top">
<p align="center"><em>quot</em> in round 4</p>
</td>
<td width="60" valign="top">
<p align="center"><em>quot</em> in round 5</p>
</td>
<td width="78" valign="top">
<p align="center">Seats won</p>
</td>
</tr>
<tr>
<td width="58" valign="top">
<p align="center">A</p>
</td>
<td width="116" valign="top">
<p align="center">70</p>
</td>
<td width="66" valign="top">
<p align="center"><strong>70</strong></p>
</td>
<td width="72" valign="top">
<p align="center">23.3</p>
</td>
<td width="60" valign="top">
<p align="center">23.3</p>
</td>
<td width="60" valign="top">
<p align="center">23.3</p>
</td>
<td width="60" valign="top">
<p align="center"><strong>23.3</strong></p>
</td>
<td width="78" valign="top">
<p align="center">2</p>
</td>
</tr>
<tr>
<td width="58" valign="top">
<p align="center">B</p>
</td>
<td width="116" valign="top">
<p align="center">60</p>
</td>
<td width="66" valign="top">
<p align="center">60</p>
</td>
<td width="72" valign="top">
<p align="center"><strong>60</strong></p>
</td>
<td width="60" valign="top">
<p align="center">20</p>
</td>
<td width="60" valign="top">
<p align="center">20</p>
</td>
<td width="60" valign="top">
<p align="center">20</p>
</td>
<td width="78" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="58" valign="top">
<p align="center">C</p>
</td>
<td width="116" valign="top">
<p align="center">50</p>
</td>
<td width="66" valign="top">
<p align="center">50</p>
</td>
<td width="72" valign="top">
<p align="center">50</p>
</td>
<td width="60" valign="top">
<p align="center"><strong>50</strong></p>
</td>
<td width="60" valign="top">
<p align="center">16.7</p>
</td>
<td width="60" valign="top">
<p align="center">16.7</p>
</td>
<td width="78" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="58" valign="top">
<p align="center">D</p>
</td>
<td width="116" valign="top">
<p align="center">30</p>
</td>
<td width="66" valign="top">
<p align="center">30</p>
</td>
<td width="72" valign="top">
<p align="center">30</p>
</td>
<td width="60" valign="top">
<p align="center">30</p>
</td>
<td width="60" valign="top">
<p align="center"><strong>30</strong></p>
</td>
<td width="60" valign="top">
<p align="center">10</p>
</td>
<td width="78" valign="top">
<p align="center">1</p>
</td>
</tr>
</tbody>
</table>
<p>The cells in bold represent the highest quotient for this seat and their party wins a seat correspondingly.</p>
<p><strong>Input Specification:</strong></p>
<p>First line of the input will contain T, the number of test cases. T test cases follow. The first line of each test case contains two integers N and S, separated by a single space. N is the number of parties and S is the number of seats to be allocated, 2&nbsp; ≤ N, S ≤ 10,000. Each of the next N lines contains the name of the party P[i], a <em>unique</em> string of at most 20 lowercase and upper case English letters, followed by a single space, then <em>an</em> integer V[i], the exact number of predicted votes to be earned by this party. 0&nbsp; ≤ V[i] ≤ 10^9 (1,000,000,000). The number of earned votes may be delimited by comas (e.g. could be 127 or 12,7). “ACM” will exist as a party name exactly once in every input case.</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, output a single line of output in the form <strong>“Case K: Method”</strong> where K is the number of the test case and Method is “S”, “D”, or “No difference”.</p>
<p>Method = “D” if <strong>D'Hondt method</strong> wins the ACM party more seats. Method = “S” if <strong>Sainte-Laguë method</strong> wins the ACM party more seats. If both methods result in the same seat count for your party, then method = “No difference”.</p>
<p><strong>Sample input:</strong></p>
<p>1</p>
<p>6 10</p>
<p>Yellow 47000</p>
<p>White 16000</p>
<p>Red 15900</p>
<p>ACM 12000</p>
<p>Blue 6000</p>
<p>Pink 3100</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: No difference</p>