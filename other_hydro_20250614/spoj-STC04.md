<p>A word consisting of N&nbsp;lower-case letters of the English alphabet ('<tt>a</tt>'-'<tt>z</tt>') is given. We would like to choose a non-empty contiguous (i.e. one-piece) fragment of the word so as to maximise the difference in the number of occurrences of the most and the least frequent letter in the fragment. We are assuming that the least frequent letter has to occur at least once in the resulting fragment. In particular, should the fragment contain occurrences of only one letter, then the most and the least frequent letter in it coincide.</p>
<h2>Input</h2>
<p>The first line of the standard input holds one integer N&nbsp;(1 &lt;= N &lt;= 10<sup>6</sup>) that denotes the length of the word. The second line holds a word consisting of N&nbsp;lower-case letters of the English alphabet.</p>
<h2>Output</h2>
<p>The first and only line of the standard output is to hold a single integer, equal to the maximum difference in the number of occurrences of the most and the least frequent letter that is attained in some non-empty contiguous fragment of the input word.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>10
aabbaaabab</pre>
<p>the correct result is:</p>
<pre>3</pre>
<p><strong>Explanation of the example:</strong>&nbsp;The fragment that attains the difference of 3 in the number of occurrences of&nbsp;<tt>a</tt>&nbsp;and&nbsp;<tt>b</tt>&nbsp;is&nbsp;<tt>aaaba</tt>.</p>