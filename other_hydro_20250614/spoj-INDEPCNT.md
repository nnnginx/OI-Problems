<p>Given integer <strong>N</strong> ( 1 &lt;= <strong>N</strong> &lt;= 60), output the number of <strong>Rooted Unlabeled Trees</strong> which have an odd number of independent sets.</p>
<p><strong>Rooted Unlabeled Tree:</strong> An Unlabeled Tree with a specified vertex as root and order amongst children does not matter. That is, two trees are considered equal if they are the same after some re-ordering of their non-root vertices. A rigorous definition is "two Rooted Unlabeled Trees T1 and T2 are equal if and only if there is a bijection <strong>f</strong> between T1 and T2 such that if root1 and root2 are the roots of T1 and T2 respectively, f(root1)=root2 and edge (u,v) is in T1 if and only if edge (f(u),f(v)) exists in T2"</p>
<p><strong>Independent Set:</strong> A set of vertices (possibly empty) is called an Independent Set if no two vertices of the set have an edge between them.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases.<br>Next T lines contain one number each, N.&nbsp;</p>
<h3>Output</h3>
<p>Output T lines, one per test case. Each line should contain the number of rooted unlabeled trees which have an odd number of independent sets. Output the answer modulo 1000000007. That is, if the actual answer is A, output A%1000000007. (This is just to keep computations within 64 bit integers.)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6</pre>
<pre>1</pre>
<pre>2</pre>
<pre>3</pre>
<pre>4</pre>
<pre>5</pre>
<pre>40</pre>
<pre><strong>Output:</strong></pre>
<pre>0</pre>
<pre>1</pre>
<pre>2</pre>
<pre>2</pre>
<pre>5</pre>
<pre>632355321</pre>