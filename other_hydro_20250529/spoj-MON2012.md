<p>Monkey Chris loves apples. That's why he has planted lots of apple trees. He does two types of operations on this trees.</p>

<ul>
<li>First operation <tt>"1 x y"</tt>: means counting ripe apple trees on interval [x+c, y+c].</li>
<li>Second operation <tt>"2 x y"</tt>: means that all apples on interval [x+c, y+c] get ripe(edible). </li>
</ul>
<p>
C=0 in the beginning and becomes the answer of each query ("1" operation). 
</p>

<h3>Input</h3>
<p>Input begins with M (1 &lt;= M &lt;= 10^5) the number of operations. Afterwards M lines each of them is an operation ("1" or "2"). 1&lt;=X+C; Y+C&lt;=10^9.</p>

<h3>Example</h3>
<pre><b>Input</b>
3
2 5 8
2 7 10
1 1 10

<b>Output</b>
6</pre>

<h3>Explanation</h3>
<p>3 queries. Apples gets ripe on intervals 5-8 and 7-10. There are totally 6 ripe apple-trees on interval 1-10 so answer to query is 6.</p>