<div>
<p><span><em>n</em></span> fish, numbered  from <span>1</span> to <span><em>n</em></span>,  live in a lake. Every day right one pair of fish meet, and the  probability of each other pair meeting is the same. If two fish with  indexes i and j meet, the first will eat up the second with the  probability <span><em>a</em><sub><em>ij</em></sub></span>,  and the second will eat up the first with the probability <span><em>a</em><sub><em>ji</em></sub> = 1 - <em>a</em><sub><em>ij</em></sub></span>. The described process goes  on until there are at least two fish in the lake. For each fish find out  the probability that it will survive to be the last in the lake.</p>
</div>
<h3>Input</h3>
<p>The first line contains integer <span><em>n</em></span> (<span>1 ≤ <em>n</em> ≤  18</span>) — the amount of fish in the lake. Then there follow <span><em>n</em></span> lines with <span><em>n</em></span> real numbers each — matrix <span><em>a</em></span>. <span><em>a</em><sub><em>ij</em></sub></span> (<span>0 ≤ <em>a</em><sub><em>ij</em></sub>  ≤ 1</span>) — the probability that fish with index <span><em>i</em></span> eats up fish with index <span><em>j</em></span>. It's guaranteed that the main diagonal  contains zeros only, and for other elements the following is true: <span><em>a</em><sub><em>ij</em></sub> = 1 -  <em>a</em><sub><em>ji</em></sub></span>. All real  numbers are given with not more than 6 characters after the decimal  point.</p>
<h3>Output</h3>
<p>Output <span><em>n</em></span> space-separated real numbers accurate to not less than 6 decimal  places. Number with index <span><em>i</em></span> should  be equal to the probability that fish with index <span><em>i</em></span> will survive to be the last in the lake.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><pre>5<br>0 1 1 1 1<br>0 0 0.5 0.5 0.5<br>0 0.5 0 0.5 0.5<br>0 0.5 0.5 0 0.5<br>0 0.5 0.5 0.5 0</pre>
<br><strong>Output:</strong> <br>
<pre>1.000000 0.000000 0.000000 0.000000 0.000000 </pre>
</pre>