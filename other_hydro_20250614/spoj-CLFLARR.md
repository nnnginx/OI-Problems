<p>You have been given an array of <strong>n</strong> unpainted elements. By unpainted, we mean that each element initially has a value of <strong>0</strong>. You have to process <strong>q</strong> queries of the form <strong>l r c</strong>, in which you paint all the elements of the array from index <strong>l</strong> to index <strong>r</strong> with color <strong>c</strong>. Assume that, each new color currently being applied to an element overrides its previous color. Output the color of each element after all the queries have been processed.</p>
<p><strong>Note</strong>: The problem is guaranteed to be solved using C or C++ programming language.</p>
<h3>Input</h3>
<p>The first line of input consists of two integers n and q. Next q lines consists of 3 integers l, r and c denoting the starting index, ending index and the color respectively.</p>
<ul>
<li>1 &lt;=&nbsp;<strong>n</strong>&nbsp;&lt;= 200000</li>
<li>1 &lt;= <strong>q</strong> &lt;= 200000</li>
<li>1 &lt;= <strong>l</strong> &lt;= <strong>r</strong> &lt;= <strong>n</strong></li>
<li>1 &lt;= <strong>c</strong> &lt;= 1 000 000 000</li>
</ul>
<h3>Output</h3>
<p>Output the final color of each element starting from index 1 on a new line.</p>
<h3>Example</h3>
<pre><strong>Input</strong>
4 3
1 3 2
2 4 6
2 3 7</pre>
<pre><strong>Output:</strong>
2
7
7
6</pre>
<pre><strong>Input</strong>
10 5
3 9 13
1 4 9
2 10 14
2 7 10
6 9 44</pre>
<pre><strong>Output</strong>
9
10
10
10
10
44
44
44
44
14</pre>