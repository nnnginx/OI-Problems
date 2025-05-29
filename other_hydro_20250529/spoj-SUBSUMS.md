<p>Given a sequence of N (1 ¡Ü N ¡Ü 34) numbers S<sub>1</sub>, ..., S<sub>N</sub> (-20,000,000 ¡Ü S<sub>i</sub> ¡Ü 20,000,000), determine how many subsets of S (including the empty one) have a sum between A and B (-500,000,000 ¡Ü A ¡Ü B ¡Ü 500,000,000), inclusive.</p>

<h3>Input</h3>
<p>The first line of standard input contains the three integers N, A, and B. The following N lines contain S<sub>1</sub> through S<sub>N</sub>, in order.</p>

<h3>Output</h3>
<p>Print a single integer to standard output representing the number of subsets satisfying the above property. Note that the answer may overflow a 32-bit integer.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 -1 2
1
-2
3

<b>Output:</b>
5
</pre>

<p>The following 5 subsets have a sum between -1 and 2:</p>
<ul>
<li>0 = 0 (the empty subset)</li>
<li>1 = 1</li>
<li>1 + (-2) = -1</li>
<li>-2 + 3 = 1</li>
<li>1 + (-2) + 3 = 2</li>
</ul>