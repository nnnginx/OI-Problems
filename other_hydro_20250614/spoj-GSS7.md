<p>Given a tree with N (<em>N</em> &lt;= 100000) nodes. Each node has a interger value x_i (<em>|x_i|</em> &lt;= 10000).</p>
<p>You have to apply Q (<em>Q</em> &lt;= 100000) operations:</p>
<p>1. <em>1 a b </em>: answer the maximum contiguous sum (maybe empty,will always larger than or equal to 0 )&nbsp;from the path <em>a-&gt;b</em> ( inclusive ).</p>
<p>2. <em>2 a b c</em> : change all value in the path <em>a-&gt;b</em> ( inclusive ) to <em>c</em>. (<em>|c|</em> &lt;= 10000)</p>
<h3>Input</h3>
<p>first line consists one interger N.</p>
<p>next line consists N interger x_i.</p>
<p>next N-1 line , each consists two interger u,v , means that node u and node v are connected</p>
<p>next line consists 1 interger Q.</p>
<p>next Q line : <em>1 a b </em>or <em>2 a b c</em> .</p>
<h3>Output</h3>
<p>For each query, output one line the maximum contiguous sum.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
-3 -2 1 2 3
1 2
2 3
1 4
4 5
3
1 2 5
2 3 4 2
1 2 5

<strong>Output:</strong>
5
9</pre>