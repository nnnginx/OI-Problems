<p>Problem statement is simple. Given <strong>A </strong>and <strong>B </strong>you need to calculate <strong>S(A,B) .</strong></p>

<p><img style="vertical-align: middle;" title="TRENDGCD problem statement" src="file://GsRVJeC6.png" alt="sigma(a=1 to A)sigma(b=1 to B) (a*b*f(gcd(a,b)))" width="512" height="102"></p>

<p>Here, <strong>f(n)=n, if n is square free otherwise 0</strong>. Also<strong> f(1)=1</strong>.</p>
<h3>Input</h3>
<p>The first line contains one integer <strong>T</strong> - denoting the number of test cases.</p>
<p><strong>T </strong>lines follow each containing two integers <strong>A,B</strong>.</p>

<h3>Output</h3>
<p>For each testcase output the value of <span style="font-weight: bold;">S(A,B) mod 1000000007 </span><span style="font-weight: bold;">in a single line</span><span style="font-weight: bold;">.</span></p>

<h3>Constraints</h3>
<ul>
<li><strong>T &lt;= 1000</strong></li>
<li><strong>1 &lt;= A,B &lt;= 1000000</strong></li>
</ul>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
42 18
35 1
20 25

<strong>Output:</strong>
306395
630
128819</pre>