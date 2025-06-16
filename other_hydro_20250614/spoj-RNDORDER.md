<p>You are given n symbols a<sub>1</sub>, a<sub>2</sub>,..., a<sub>n</sub>. You are told that there is a total ordering of the symbols. That is, there is a permutation [P1, P2,..., Pn] of [1,2,...,n] such that a<sub>P1</sub>&lt; a<sub>P2 </sub>&lt;...&lt; a<sub>Pn</sub>. You are trying to figure out the order by doing comparisons. The process you follow for determining the order is as follows:</p>
<ul>
<li>Compare [a<sub>1</sub>, a<sub>2</sub>]</li>
<li>Compare [a<sub>2</sub>, a<sub>3</sub>], [a<sub>1</sub>, a<sub>3</sub>]&nbsp;</li>
<li>Compare [a<sub>3</sub>, a<sub>4</sub>], [a<sub>2</sub>, a<sub>4</sub>], [a<sub>1</sub>, a<sub>4</sub>]</li>
<li>....</li>
<li>....</li>
<li>Compare [a<sub>n-1</sub>,a<sub>n</sub>], [a<sub>n-2</sub>,a<sub>n</sub>],..., [a<sub>1</sub>, a<sub>n</sub>]</li>
</ul>
<p>Note that you compare in the order specified. That is you compare [a<sub>2</sub>, a<sub>3</sub>], then and only then do you compare [a<sub>1</sub>, a<sub>3</sub>].</p>
<p>Definition of Compare[a<sub>i</sub>, a<sub>j</sub>] (i &lt; j)</p>
<ul>
<li>If Compare [a<sub>i</sub>, a<sub>j</sub>] = 1, it means a<sub>i</sub> &gt; a<sub>j</sub>. If Compare[a<sub>i</sub>, a<sub>j</sub>] = -1, it means a<sub>i</sub> &lt; a<sub>j</sub>.&nbsp;</li>
<li>Compare is consistent. Suppose, that you queried [a<sub>2</sub>, a<sub>6</sub>] and it was already established [a<sub>2</sub> &lt; a<sub>6</sub>] (because for example a<sub>2</sub> &lt; a<sub>5</sub> and a<sub>5</sub> &lt; a<sub>6</sub> - since both of these comparisons happen earlier), then [a<sub>2</sub>, a<sub>6</sub>] returns -1.</li>
<li>If no relationship is known between a<sub>i</sub> and a<sub>j</sub>, Compare[a<sub>i</sub>, a<sub>j</sub>] = 1 with probablity 1/2 and -1 with probability 1/2</li>
</ul>
<p>Your task is to output the probability that a<sub>1</sub> is the smallest element of the final ordering so obtained.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases</p>
<p>Each of the next T lines contains one number each, <strong>n</strong>(1 &lt;= n &lt;= 1000).&nbsp;</p>
<h3>Output</h3>
<p>Output T lines in total, one per test case: Probability that a<sub>1</sub> is indeed the smallest element at the end of the comparisons. Your output will be judged correct if it differs by no more than 10<sup>-9</sup> to the reference answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3</pre>
<pre>1</pre>
<pre>2</pre>
<pre>3

<strong>Output:</strong>
</pre>
<pre>1</pre>
<pre>0.500</pre>
<pre>0.3750000</pre>
<pre><strong>Explanation:</strong></pre>
<pre>n = 1 is trivial</pre>
<pre>For n = 2, only comparison is [a<sub>1</sub>, a<sub>2</sub>]. a1 is lower with probability 1/2.</pre>
<pre>For n = 3, a1 is not the least element if either (a<sub>1</sub> &gt; a<sub>2</sub>) or (a<sub>1</sub> &lt; a<sub>2</sub> and a<sub>3</sub> &lt; a<sub>2</sub> and a<sub>3</sub> &lt; a<sub>1</sub>).&nbsp;</pre>
<pre>So, probability that a<sub>1</sub> is not the least element = 1/2 + 1/8 = 5/8. Probability that a<sub>1</sub> is the least = 3/8 = 0.375.</pre>