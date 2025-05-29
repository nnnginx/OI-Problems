<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;Deisy is working on a robotics project, she wants to test the robot at the top before sending it to a very important company, she made a complete map for the robot, the robot is in the beta test, so it's a little dummy, the robot can't walk in diagonals, it only can walk in four directions; north, south, east or west, Deisy thinks someway this is a very bad thing, so, she wants to know if a diagonal is always the <strong>best</strong> path for the robot to go through.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">You are going to test the robot's diagonal steps versus the real steps the robot can make from a <em>map A to a map B</em>, having in consideration that the robot can start whenever in map A or B and arrives to the nearest point in B or A, also, Deisy can choose any point as a start for the robot (this point will belong to a map) and you must <strong>not</strong> compare the set of points where the robot belongs.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Definition of a "map": a map is a set of stars (*) in adjacency, we define the adjacency as the four positions (north,south,east,west), meaning that a star is adjacent to other if they are communicated by one of these positions.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>INPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">The first line of input will contain an integer T denoting the T test cases, then, T cases will follow. Each of the following cases will contain a line with an integer N, then N lines with N characters each will follow, denoting the map the robot will have to traverse from a set of points A to a set of points B, a free space will be denoted by '-' and a occupied space by some point will be denoted by a character '*', it is guaranteed that there will be always two maps.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>OUTPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Output the string ¡°Scenario #i: ¡° where i is the test case you are analyzing followed by the option to choose, output 1 if the robot can go by its normal direction, 0 if going in diagonals is better.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">SAMPLE DATA:</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><strong>INPUT</strong></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><strong>OUTPUT</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="JUSTIFY">2</p>
<p align="JUSTIFY">5</p>
<p align="JUSTIFY">---**</p>
<p align="JUSTIFY">---**</p>
<p align="JUSTIFY">-----</p>
<p align="JUSTIFY">**---</p>
<p align="JUSTIFY">**---</p>
<p align="JUSTIFY">4</p>
<p align="JUSTIFY">*--*</p>
<p align="JUSTIFY">*--*</p>
<p align="JUSTIFY">*--*</p>
<p align="JUSTIFY">*--*</p>
<p align="JUSTIFY">&nbsp;</p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="JUSTIFY">Scenario #1: 0</p>
<p align="JUSTIFY">Scenario #2: 1</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Explanation of the first case: For each point in the matrix either you start in map A or B, traversing in diagonals will always be better, the output should be zero (0).</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Note: if Deisy find herself with equal distance between the diagonal and the "normal" steps of the robot, she will choose the "normal" steps as the best, in this case, the output should be 1 (normal is better).</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>CONSTRAINTS:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">2&lt;=N&lt;=1000</p>