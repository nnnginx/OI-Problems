Let <b>A</b> and <b>B</b> be two strings made up of alphabets such that <b>A = A<sub>[1-n]</sub>, B = B<sub>[1-m]</sub></b>. We say <b>B</b> is a subsequence of <b>A</b> if there exists a sequence of indices  <b>i<sub>1</sub> &lt; i<sub>2</sub> &lt;..<i<sub>m</i<sub></b> of <b>A</b> such that <b>A[i<sub>k</sub>] = B[k]</b>. 
<p></p>

<p>
Given <b>B[1-m]</b>, a string of characters from some alphabets, <b>B^i</b> is defined as string with the characters of <b>B</b> each repeating <b>i</b> times. For example, <b>(abbacc)^3 = aaabbbbbbaaacccccc</b>.
Also, <b>B^<font face="courier">0</font></b> is the empty string.
</p>

<p>
Given strings <b>X</b>, <b>Y</b> made up of characters from <b>'a' - 'z'</b> find the maximum value of <b>M</b> such that <b>X^M</b> is a subsequence of <b>Y</b>.
</p>

<h3>Input</h3>

<p>
</p><ul>
<li> The first line of the input contains a positive integer <b>t &lt;= 20</b>, denoting the no. of test cases.
</li><li> The following <b>2t</b> lines contain the value of <b>X</b> and <b>Y</b> for the cases.
</li><li> The description of the test cases follow one after the other.
<ul>
<li> Line <b>2k</b> contains the value of <b>X</b> for case <b>k</b>; <b>(1 &lt;= k &lt;= t)</b>
</li><li> Line <b>2k+1</b> contains the value of <b>Y</b> for case <b>k</b>; <b>(1 &lt;= k &lt;= t)</b>.
</li><li> The no. of characters in <b>X</b> , <b>Y</b> will be  <b>&lt;= 500010</b>.
</li></ul>
</li></ul>

<h3>Output</h3>
<p>
The output must contain <b>t</b> lines, each line corresponding to a test case.
The value on the <b>k<sup>th</sup></b> line should be the value of <b>M</b> for the <b>k<sup>th</sup></b> pair of <b>X</b> and <b>Y</b>. 
</p>
 
<p>
</p><h3>Example</h3>

<p><tt>
<b>Input:</b>
<br>3
<br>abc
<br>aabbcc
<br>abc
<br>bbccc
<br>abcdef
<br>abc
</tt></p><tt>

</tt><p><tt>
<b>Output:</b>
<br>2
<br>0
<br>0
</tt>
</p>