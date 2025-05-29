<p>Given two arrays A and B of size n and x.Apoorv is given an empty array P.He has to fill the array according to the following conditions:</p>
<pre>for each i in range (0 to x-1){
</pre>
<pre>if b[i] is negative (insert the subarray from A[abs(B[i]] to A[n-1] in P at the end)
</pre>
<pre>else  (insert the subarray from A[0]to A[B[i]] in P at the end)
</pre>
<pre>}</pre>
<p>Since Apoorv loves Prime numbers He wants to know the Kth prime number in P after the above operation is completed.</p>
<p>So given q queries Apoorv has to report the kth prime number in it.If kth prime doesn't exist print -1.</p>
<p>&nbsp;</p>
<p>Note:Both A and B are 0 indexed.abs stands for absolute value.</p>
<p>Constraints:</p>
<p>1&lt;=n&lt;=100000</p>
<p>1&lt;=x&lt;=100000</p>
<p>1&lt;=A[i]&lt;=1000000</p>
<p>0&lt;=abs(B[i])&lt;=n-1</p>
<p>1&lt;=q&lt;=10000</p>
<p>1&lt;=k&lt;=10000000000</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line will contain n size of A.</p>
<p>Second line will contain n space separated integers denoting A[i].</p>
<p>Third line will contain x denoting size of B.</p>
<p>Fourth line will contain&nbsp;x space separated integers denoting B[i].</p>
<p>Fifth line will contain q denoting number of queries.</p>
<p>Sixth line will contain q space separated integers denoting k.</p>
<h3>Output</h3>
<p>Print q lines denoting output for each query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
</pre>
<pre>2 3 4</pre>
<pre>1</pre>
<pre>2</pre>
<pre>3</pre>
<pre>1 2 3</pre>
<pre><strong>Output:</strong>
</pre>
<pre>2</pre>
<pre>3</pre>
<pre>-1</pre>
<pre>Explanation : P is [2,3,4] so for k=1 answer is 2 ,for k=2 answer is 3,for k=3 answer=-1 because 3rd prime number doesn't  exist.
</pre>