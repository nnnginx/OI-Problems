<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Bobs just got an array A of n integers from his mother Ksenxi. She asked him to calculate the goodness of A.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Let's define f(a, b) of A as minimum value on interval [a, b] in A.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 ≤ a ≤ b &lt; c ≤ d ≤ n and f(a, b) ≤ f(c, d).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Since Bobs is writing esay on matura in few days he is now reading short summaries of books on mandatory the reading list so he needs your help to answer his mom this hard question.</div>
<p>Bobs just got an array A of <strong><em>n</em></strong> integers from his mother Ksenxi. She asked him to calculate the goodness of A.&nbsp;</p>
<p>Let's define f(a, b) of A as minimum value on interval [a, b] in A. &nbsp;<br>Goodness of A is the number of pairs of segments [a, b], [c, d] such that<strong> <br>1</strong> ≤<strong> </strong>a<strong> </strong>≤ b &lt; c ≤ d ≤<strong> <em>n</em> </strong>and f(a, b) ≤ f(c, d).</p>
<p>Since Bobs is writing an essay on matura in a few days he is now reading short summaries of books on the mandatorys reading list&nbsp;so he needs your help to answer this hard question to his mom.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong><em>n</em></strong> (<strong>1</strong> ≤ <em><strong>n</strong></em> ≤ <strong>500000</strong>).<br>The second line contains n space-saparated integers A<sub>1</sub>, A<sub>2</sub>, ..., A<sub>n</sub> (<strong>0</strong> ≤ A<sub>i</sub> ≤ <strong>10<sup>9</sup></strong>) - the array elements.</p>
<h3>Output</h3>
<p>Print out a single integer - the goodness of A. As the answer can be quite a large number, you should print it modulo <strong>10<sup>9</sup> + 7 </strong>(<strong>1000000007</strong>).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
5 3 0 9 8 

<strong>Output:</strong>
21
</pre>