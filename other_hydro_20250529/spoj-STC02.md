<p>Byteasar studies certain strings of zeroes and ones. Let S&nbsp;be such a string. By S<sup>r</sup>&nbsp;we will denote the reversed (i.e., "read backwards") string S, and by S<sup>I</sup>&nbsp;we will denote the string obtained from S&nbsp;by changing all the zeroes to ones and ones to zeroes.</p>
<p>Byteasar is interested in&nbsp;<em>antisymmetry</em>, while all things symmetric bore him. Antisymmetry however is not a mere lack of symmetry. We will say that a (nonempty) string S&nbsp;is&nbsp;<em>antisymmetric</em>&nbsp;if, for every position i&nbsp;in S, the i-th last character is different than the i-th (first) character. In particular, a string S&nbsp;consisting of zeroes and ones is antisymmetric if and only if S=S<sup>Ir</sup>. For example, the strings&nbsp;<tt>00001111</tt>&nbsp;and&nbsp;<tt>010101</tt>&nbsp;are antisymmetric, while&nbsp;<tt>1001</tt>&nbsp;is not.</p>
<p>In a given string consisting of zeroes and ones we would like to determine the number of contiguous nonempty antisymmetric fragments. Different fragments corresponding to the same substrings should be counted multiple times.</p>
<h2>Input</h2>
<p>The first line of the standard input contains an integer N&nbsp;(1 &lt;= N &lt;= 500000) that denotes the length of the string. The second line gives a string of 0 and/or 1 of length N. There are no spaces in the string.</p>
<h2>Output</h2>
<p>The first and only line of the standard output should contain a single integer, namely the number of contiguous (non empty) fragments of the given string that are antisymmetric.</p>
<p>&nbsp;</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>8
11001011</pre>
<p>the correct result is:</p>
<pre>7</pre>
<p>Antisymmetric fragments are:&nbsp;<tt>01</tt>&nbsp;(occurs twice),&nbsp;<tt>10</tt>&nbsp;(also twice),&nbsp;<tt>0101</tt>,&nbsp;<tt>1100</tt>, and&nbsp;<tt>001011</tt>.</p>