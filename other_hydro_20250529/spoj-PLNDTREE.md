<pre><span style="white-space: normal;"><span style="font-size: medium;"><p>John has got a tree with N vertices. The vertices are numbered from 1 to N. He considers vertex 1 as the root of the tree. Each vertex of the tree contains a character C.</p>
<p>Now John is doing a weird experiment with this tree.</p>
<p>He often changes the character of a node in the tree and then sometimes he randomly selects a node v and tries to form a palindrome with all the characters in the subtree of node v.</p>
<p>But since John is very busy man and has a lot of other important experiments to do he needs your help on this one.</p>
<p><strong><span style="text-decoration: underline;">INPUT:</span></strong></p>
<p>First line of the input contains an integer N (1&lt;=N&lt;=100000) denoting the number of vertices.</p>
<p>Next N-1 lines contains two integers A and B (1&lt;=A, B&lt;=N) which means there is an edge between vertex A and B.</p>
<p>Next line contains a string of length N. The ith character of this string denotes the character in node i.</p>
<p>Then there will be an integer M (1&lt;=M&lt;=100000) in a separate line denoting the number of queries. Next M lines will contain a query.</p>
<p>Each query will be in one of the following form:<strong>&nbsp;</strong></p>
<p><strong>0 x C</strong>: which means the character of node x has been changed to C.<strong>&nbsp;</strong></p>
<p><strong>1 x:&nbsp;</strong>which means you are asked to answer if a palindrome can be formed with all the characters in the sub tree of node x. There will be at least one query of this type.</p>
<p><strong><span style="text-decoration: underline;">OUTPUT:</span></strong></p>
<p>For each query of the form&nbsp;<strong>¡°1 x¡±&nbsp;</strong>print ¡°YES¡± if a palindrome can be formed with all the characters in subtree of node x. Otherwise print ¡°NO¡± (without the quotes).</p>
<p>(All the characters in the input will be small letters of English alphabet. i.e. a, b, c¡­ x, y, z).</p>
<p>See sample input /sample output for details.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="312" valign="top">
<p><strong><span style="text-decoration: underline;">Sample   Input</span></strong></p>
</td>
<td width="312" valign="top">
<p><strong><span style="text-decoration: underline;">Sample   Output</span></strong></p>
</td>
</tr>
<tr>
<td width="312" valign="top">
<p>7</p>
<p>5 4</p>
<p>1 5</p>
<p>6 3</p>
<p>1 7</p>
<p>5 6</p>
<p>6 2</p>
<p>abdaabc</p>
<p>7</p>
<p>1 1</p>
<p>1 5</p>
<p>1 3</p>
<p>0 7 a</p>
<p>1 1</p>
<p>0 4 z</p>
<p>1 5</p>
</td>
<td width="312" valign="top">
<p>NO</p>
<p>YES</p>
<p>YES</p>
<p>YES</p>
<p>NO</p>
<p>&nbsp;</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>In the 2<sup>nd</sup>&nbsp;query, the formed palindrome can be ¡°badab¡± or ¡°abdba¡±</p>
<p>In the 3<sup>rd</sup>&nbsp;query, there is only 1 character ¡°d¡±, which is palindrome.</p>
<p>&nbsp;</p></span></span></pre>