<pre><span style="white-space: normal;"><p>After Johnny spent a long day in school, he decided to play a spot game with his friends. A Spot game is played as follows, there are <strong><em>N</em></strong> spots on a horizontal line one after another, each spot <strong><em>i</em></strong> has a radius <strong><em>R[i]</em></strong>. The player may start at any spot, but is only allowed to move from one spot to another if it occurs after it in the line and its radius is greater than the previous one. When he plays a move on a spot <strong><em>i</em></strong> he earns <strong><em>P[i]</em></strong> points. The player wins when he goes through the maximum number of spots if there are multiple ways, He must earn the maximum sum of points, if there are still multiple ways he must select the one that is lexicographically maximal (Let A=(a1,...,aN) and B=(b1,...,bN) be two different but equally large solution, with a1 &gt;= a2 &gt;= ... &gt;= aN and b1 &gt;= b2 &gt;= ... &gt;= bN. Let x be the smallest index such that ax != bx. If ax &gt; bx, we say that the set A is lexicographically larger than the set B). As Johnny is a smart boy he wants to play optimally, so he asked you to show him which spots to move in order to win the game, Can you help him?&nbsp;</p>
<h2>Input Format</h2>
<p>Input will start with <strong><em>T</em></strong> number of test cases. Each test case starts with <strong><em>N</em></strong> where 1 &lt;= <strong><em>N </em></strong>&lt;= 1500 represent number of spots. Then follow <strong><em>N</em></strong> lines each contains two integers <strong><em>R[i]</em></strong> and <strong><em>P[i]</em></strong> where 1 &lt;= <strong><em>R[i] </em></strong>&lt;= 300 is the radius of <strong><em>i</em></strong>-th spot and 1 &lt;= <strong><em>P[i] </em></strong>&lt;= 2,000,000 is the points earned when you move on <strong><em>i</em></strong>-th spot.</p>
<h2>Output Format</h2>
<p>For each test case, output the result using the following format:</p>
<p><strong><em>K</em></strong> (start with 1) followed by a period, and a single space, then print the indices (1-based) of the spots that Johnny visits separated by a single space. If there are more than one subsequence of spots that makes Johnny wins then print the lexicographically largest.</p>
<p>&nbsp;</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="284" valign="top">
<h2>Sample Input</h2>
</td>
<td width="284" valign="top">
<h2>Sample Output</h2>
</td>
</tr>
<tr>
<td width="284" valign="top">
<p>2</p>
<p>6<br> 1 3<br> 2 3<br> 6 3<br> 4 20 <br> 3 15<br> 9 10<br> 6<br> 1 3<br> 1 3<br> 6 3<br> 4 20<br> 3 15<br> 9 10</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="284" valign="top">
<p>1. 1 2 4 6</p>
<p>2. 2 4 6</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p></span></pre>