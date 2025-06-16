<p>As you know, after the award ceremony of SWERC it is customary to publish a complete scoreboard with detailed information on the submissions and verdicts received. However, due to the buggy contest management system, most of the relevant data are not being recorded today. Clearly such state of affairs fails to meet the high standards we are committed to, so the judges have resolved to make up the rest of the data based on whatever shred of information left, and hope contestants are unable to tell the difference. To make our lives even simpler, we kindly ask you to provide a solution for us, or else today��s scoreboard will remain forever veiled in mystery (even the fake one).</p>
<p>What we will know by the end of the contest is the number <em>T</em> of teams, the number <em>P</em> of problems, and the number of accepted submissions by each team. From the number and colour of balloons floating around on the premises we will also be able to infer how many teams solved each of the problems. Your task is to figure out which teams solved which problems.</p>
<p>Our counting skills are not up to par, so your program should be able to detect when the data we collected must be wrong (see sample input 1). Otherwise you should output a possible solution, represented as a sequence of <em>T</em> strings of <em>P</em> characters each, in the following way. Both problems and teams are assigned with distinct integers, from 1 to <em>P</em> and 1 to <em>T</em>, respectively. For team number <em>i</em> (1 �� <em>i</em> �� <em>T</em>), write the string on alphabet <tt>N,Y</tt> such that its <em>j</em>-th (1 �� <em>j</em> �� <em>P</em>) character is <tt>Y</tt> if the team managed to get problem <em>j</em> accepted, and <tt>N</tt> otherwise.  For example, the following three strings form a solution to the second sample case, where the score of each of three teams is 2,1,2, and the count of accepted submissions for each of three problems is 1,2,2:</p>
<table class="display dcenter" border="0">
<tbody>
<tr valign="middle">
<td class="dcell">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="center"><tt>NYY</tt></td>
</tr>
<tr>
<td align="center"><tt>NNY</tt></td>
</tr>
<tr>
<td align="center"><tt>YYN</tt></td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>There is at least one other solution, namely</p>
<table class="display dcenter" border="0">
<tbody>
<tr valign="middle">
<td class="dcell">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="center"><tt>NYY</tt></td>
</tr>
<tr>
<td align="center"><tt>NYN</tt></td>
</tr>
<tr>
<td align="center"><tt>YNY</tt></td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>When several solutions are possible we ask you to supply the one giving rise to the lexicographically smallest string, when each of the <em>T</em> rows are concatenated in order. In the example above we prefer the first solution, since <tt>NYYNNYYYN</tt> comes before <tt>NYYNYNYNY</tt> in lexicographical order. (String <em>S</em> comes before <em>S</em>�� in lexicographical order if the first different character between the two is <tt>N</tt> in <em>S</em> but <tt>Y</tt> in <em>S</em>��).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each input case is described by three lines:</p>
<p>The first contains two space-separated integers <em>T</em> (the number of teams) and <em>P</em> (the number of problems), with 1 �� <em>T</em>, <em>P</em> �� 80. The second contains <em>T</em> space-separated integers between 0 and 90 (inclusive), the <em>i</em>-th of which indicates the number of problems solved by team <em>i</em>. The third (and last) line has <em>P</em> integers between 0 and 90, the <em>j</em>-th of which describes the number of teams successfully solving problem <em>j</em>.</p>
<p>Different input cases are separated by a blank line. The last line of the input file will be <tt>0 0</tt>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>If the input data has a solution, print <em>T</em> lines of <em>P</em> characters each, depicting the lexicographically smallest solution as explained above. Otherwise output a single line with the word <tt>Impossible</tt>. In any case a blank line should separate outputs for different test cases.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2 2
1 2
1 1

3 3
2 1 2
1 2 2

3 5
3 3 1
3 1 1 0 2

0 0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">Impossible

NYY
NNY
YYN

YNYNY
YYNNY
YNNNN
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David Garc��a Soriano</em></blockquote>