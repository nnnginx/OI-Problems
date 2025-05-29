<p>
You are given N numbers  of the array (N &lt;= 100000), all less than 10^8 and greater than 0.
</p>
<p>
Now, you are given 2 queries:
</p>
<ol>
  <li><tt>"1 x i"</tt> : Change the i-th number to x. (0 &lt;= x &lt;= 10^8)</li>
  <li><tt>"2 Op i1 i2"</tt>: Compute the sum of all two elements taken at a time within index i1 to i2(both inclusive) under the operation Op.
Op could be XOR,OR or AND.</li>
</ol>
<p>For example, let N=4, Query=3 and <tt>"10 20 30 40"</tt> be the Initial array.</p>

<p>Query:</p>
<pre>2 OR 1 3
1 0 1
2 OR 1 3
</pre>

<p>Answer:</p>

<pre>2 OR 1 3--&gt; (10 OR 20) + (20 OR 30) + (10 OR 30)
1 0 1   --&gt; Now array becomes 0 20 30 40
2 OR 1 3--&gt; (0 OR 20) + (20 OR 30) + (0 OR 30)</pre>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 3
10 20 30 40
2 OR 1 3
1 0 1
2 OR 1 3

<strong>Output</strong>
90
80</pre>

<p><strong>NOTE:</strong> If i1 is equal to i2, always output 0.</p>
<p><a href="../../problems/INTRO/">Click here to see my set of problems at Spoj.</a></p>