<p>"Why me?" ,zing asked.</p>
<p>"If you're a star then I'm the darkness.You complete me ",he replied.</p>
<p>Being impressed by him, she gave him an another task.</p>
<p>Build a tree with following rules:</p>
<ul>
<li>If a node with (l,r) is given</li>
<li>Break it into left node with (l,mid)</li>
<li>Break it into right node with (mid+1,r)</li>
<li>stop when leaf node appears (l=r)</li>
</ul>
<p>where mid=(l+r)/2.</p>
<p>So count the number of leaf nodes which do not appear in pairs.</p>
<p>For more clarification,see examples below.</p>
<h3>Input</h3>
<p>Line 1: No. of queries (&lt;=100000)</p>
<p>Line 2: In next q lines , l r is given (0&lt;=l&lt;=r&lt;=10^18)&nbsp;</p>
<h3>Output</h3>
<p>For every query, print the answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>2 4</pre>
<pre>4 5</pre>
<pre><strong>Output:</strong>
1</pre>
<pre>0</pre>
<pre>Explanation : In (2,4) --&gt; (2,3) and (4,4)</pre>
<pre>                        (2,3) --&gt; (2,2) and (3,3)</pre>
<pre>                        Here (4,4) is the only leaf node which did'nt appear in pair.</pre>