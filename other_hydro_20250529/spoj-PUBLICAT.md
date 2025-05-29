<p>The Orizondo number is a way of describing the "collaborative distance" between a scientist and Rodrigo Orizondo by authorship of scientific publications. <br><br>Rodrigo Orizondo is the only person who has an Orizondo number equal to zero. To be assigned a finite Orizondo number, a scientist must publish a paper in co-authorship with a scientist with a finite Orizondo number. The Orizondo number of a scientist is the lowest Orizondo number of his coauthors + 1. The order of publications and numbers assignment doesn't matter, i.e., after each publication the list of assigned numbers is updated accordingly. <br><br>You will be given the <strong>publications</strong>, each element of which describes the list of authors of a single publication and is formatted as "AUTHOR_1 AUTHOR_2 ... AUTHOR_N" (quotes for clarity only). Rodrigo Orizondo will be given as "ORIZONDO". <br><br>Print out the list of Orizondo numbers which will be assigned to the authors of the listed publications. Each element of the printout should be formatted as "AUTHOR NUMBER" if AUTHOR can be assigned a finite Orizondo number, and just "AUTHOR" otherwise. The authors in the printout list must be ordered lexicographically.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases <em>C</em> (<em>0 &lt; C ¡Ü 10,000</em>).</p>
<p>Each test case starts with an integer N, the number of publications, then N publications follow. Each publication consists in a space separated list of authors.(each publication in a single line).</p>
<table border="0">
<tbody>
<tr>
<td colspan="2">
<h3><span style="font-size: x-small;">Notes</span></h3>
</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>All authors mentioned in the list must be present in output.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>Assume that all publications of mentioned authors are given in <strong>publications</strong>.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>String S is lexicographically before string T if S is a proper prefix of T, or if S has an earlier character at the first position where the strings differ.</td>
</tr>
<tr>
<td colspan="2">&nbsp;</td>
</tr>
<tr>
<td colspan="2">
<h3><span style="font-size: x-small;">Constraints</span></h3>
</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td><strong>publications</strong> will contain between 1 and 50 elements, inclusive.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>Each element of <strong>publications</strong> will contain between 1 and 50 characters, inclusive.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>An author is a string of between 1 and 50 uppercase letters ('A'-'Z'), inclusive.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>Each element of <strong>publications</strong> will be a list of authors, separated by single spaces.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>Each element of <strong>publications</strong> will not have any trailing spaces.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>The authors in each element of <strong>publication</strong> will be distinct.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>There will be at most 100 distinct authors in all publications.</td>
</tr>
<tr>
<td align="center" valign="top">-</td>
<td>Rodrigo Orizondo will be given as "ORIZONDO", and at least one publication will list him as one of the authors.</td>
</tr>
</tbody>
</table>
<h3>Output</h3>
<p>For each test case, output one line containing each author with his Orizondo Number, all space separated.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>1<br>ORIZONDO<br>2<br>KLEITMAN LANDER<br>ORIZONDO KLEITMAN<br>4<br>ORIZONDO B<br>A B C<br>B A E<br>D F<br><br><br><strong>Output:</strong><br>ORIZONDO 0<br>KLEITMAN 1 LANDER 2 ORIZONDO 0<br>A 2 B 1 C 2 D E 2 F ORIZONDO 0<br></pre>