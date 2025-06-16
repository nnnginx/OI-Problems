<p><span style="color: #222222; font-family: arial, sans-serif; font-size: 13px;">Taplu and Abhishar loved playing scrabble. One day they thought of inventing a new game using alphabet tiles. Abhishar wrote a string using tiles and gave a set of pairs (i,j) to Taplu. Pair ¡°i, j¡± (0 based indexing) means that Taplu can swap the i¡¯th and j¡¯th tile in the string any number of times.</span><span style="color: #222222; font-family: arial, sans-serif; font-size: 13px;">&nbsp;&nbsp;</span><span style="color: #222222; font-family: arial, sans-serif; font-size: 13px;">He then asks Taplu to give the lexicographically smallest string that can be produced by doing any number of swaps on the original string.</span></p>
<h3>Input</h3>
<p>First line contains T(1&lt;=T&lt;=10), the number of testcases.</p>
<p>First line of each test case contains the initial string S. Length of Sttring is len(1&lt;=len&lt;=100000).</p>
<p>Next line contains the number of pairs M (1&lt;=M&lt;=100000).</p>
<p>Next M lines contains pairs i j that means ith character can be swapped with jth character.</p>
<p>Note - i and j can be same and same i,j pair can occur twice.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each testcase output the lexicographically smallest string that can be made from the initial string.</p>
<h3>Example</h3>
<pre><strong>Input:<br><br></strong>1<strong><br></strong>lmaf<br>3<br>0 1<br>1 2<br>2 3

<strong>Output:</strong>
aflm
</pre>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Suppose you are given a string of length n and a set of pairs(i, j such  that 0 &lt;= i &lt; j &lt; n). Pair ¡°i, j¡± (0 based indexing) means that  you can swap the i¡¯th and j¡¯th character in the string any number of  times. You have to output the lexicographically smallest string that can  be produced by doing any number of swaps on the input string.</div>