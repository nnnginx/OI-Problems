<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given a sequence of N(1&lt;=N&lt;=1000000) numbers range from 0 to 10000 and several other sequence of M(0&lt;=M&lt;=5) numbers, you have to compute the Longest Common Subsequence of this sequences with the main sequence.</div>
<p>&nbsp;</p>
<p>Given a main sequence of N(1&lt;=N&lt;=1000000) numbers range from 0 to 10000 and several other sequence of M(0&lt;=M&lt;=5) numbers, you have to compute the Longest Common Subsequence of this sequences with the main sequence.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line of the input will be N the number of elements of the main sequence. After that line there will be N numbers in one or more lines. Each of this number will be between 0 to 10000(inclusive). Then there will be Q(1&lt;=Q&lt;=5000) the number of query. Then following Q lines will be queries. In each query, start with a number M(0&lt;=M&lt;=5), followed by M numbers also between 0 to 10000(inclusive).</p>
<h3>Output</h3>
<p>For each query first print the number of elements in the longest common subsequence of the main and query sequences. Then print the subsequence. If there is more then one then print the lexicographically smallest.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10</pre>
<pre>5 1 4 3 2 6 5 5 0 7</pre>
<pre>5</pre>
<pre>1 5</pre>
<pre>1 10</pre>
<pre>4 5 0 4 7</pre>
<pre>5 4 1 2 3 5</pre>
<pre>5 2 6 5 0 7</pre>
<p>&nbsp;</p>
<pre><strong>Output:</strong>
1 5
0
3 5 0 7
3 1 2 5
5 2 6 5 0 7<span style="white-space: normal;">
</span></pre>
<pre></pre>
<pre><strong>Huge Test Case<span style="color: #000020;"><span style="white-space: normal; -webkit-border-horizontal-spacing: 2px; -webkit-border-vertical-spacing: 2px;">(Almost 5MB)</span></span></strong></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>