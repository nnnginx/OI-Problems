<p>Given a sequence S of N integers, indexed from 0 to N-1, we define the weight of its continuous subsequence as the product of its length and its number of occurrences in the main sequence, and in case of uniqueness, we say its weight is 0.<br><br>&nbsp;&nbsp; Let's see an example:<br><br>&nbsp;&nbsp; N = 5<br>&nbsp;&nbsp; S = { 1, 7, 3, 1, 7 }</p>
<p>The continuous subsequence S[ 0, 1 ], which is equal to { 1, 7 }, has a weight of 4, by definition. The continuous subsequence S[ 2, 2 ] thus has a weight of 0.</p>
<p>Your task is to find the continuous subsequence of maximum weight. To break ties, choose the lexicographically smallest of the candidates ( a sequence A is lexicographically smaller than another sequence B if the first element at which they differ is smaller in A, or if A is a prefix of B ).<br><br>If the maximum weight of all the continuous subsequences is 0, we say the sequence is invalid.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer, N ( 1 &lt;= N &lt;= 10<sup>5</sup> ).<br>The second line of input contains a sequence S of N integers, ( 0 &lt;= S<sub>i</sub> &lt;= 10<sup>9</sup> ).</p>
<h3>Output</h3>
<p>In case of an invalid subsequence, output -1.<br>A continuous subsequence of the input sequence with the property defined above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5<br>1 7 3 1 7<br>&nbsp;<br><strong>Output:</strong><br>1 7</pre>