<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MINMOVE/en/">English</a></td>
<td width="50%"><a href="/problems/MINMOVE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p> </p>
<p>Given a string S[1..n] . A rotation on S is that we move the first character to the right-most of the string. More specific, after a rotation, S becomes T = S[2..n] + S[1].</p>
<p>For example: S = abcaa, then after a rotation we have S = bcaaa.</p>
<p>Find the minimum number of rotations to make S become the smallest lexicographical order string.</p>
<h3>Input</h3>
<p>A single line contains a string S. S contains only small letters of English alphabet (¡®a¡¯ .. ¡®z¡¯), and the length of S is not more than 100000.</p>
<h3>Output</h3>
<p>A single line contains an integer which represents the minimum number of rotations.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
mississippi

<strong>Output:</strong>
10

</pre>
<p><strong>Test cases and time limit have been updated. Some accepted solution got TLE.</strong> </p>