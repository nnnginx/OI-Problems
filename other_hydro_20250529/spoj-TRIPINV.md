<p>The n^2 upper bound for any sorting algorithm<br>is easy to obtain: just take two elements<br>that are misplaced with respect to each other<br>and swap them. Conrad conceived an algorithm<br>that proceeds by taking not two, but three misplaced<br>elements. That is, take three elements<br>ai &gt; aj &gt; ak with i &lt; j &lt; k and place them in<br>order ak; aj ; ai. Now if for the original algorithm<br>the steps are bounded by the maximum number<br>of inversions n(n-1)/2, Conrad is at his wits' end as<br>to the upper bound for such triples in a given sequence. He asks you to write a program<br>that counts the number of such triples.</p>
<h3>Input</h3>
<p>The rst line of the input is the length of the sequence, 1 &lt;= n &lt;= 10^5.<br>The next line contains the integer sequence a1; a2..an.<br>You can assume that all ai belongs [1; n].</p>
<h3>Output</h3>
<p>Output the number of inverted triples.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>3 3 2 1
<strong>Output:</strong>
2
</pre>