<p>
</p><p>You are given an undirected graph G(V, E). Each vertex has a mark which is an integer from the range [0..2<sup>31</sup> ¨C 1]. Different vertexes may have the same mark.</p>

<p>For an edge (u, v), we define Cost(u, v) = mark[u] xor mark[v].</p>

<p>Now we know the marks of some certain nodes. You have to determine the marks of other nodes so that the total cost of edges is as small as possible.</p>
<p></p>

<h3>Input</h3>
<p>The first line of the input data contains integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 10) - the number of testcases. Then the descriptions of T testcases follow.</p>

<p>First line of each testcase contains 2 integers <b>N</b> and <b>M</b> (0 &lt; <b>N</b> &lt;= 500, 0 &lt;= <b>M</b> &lt;= 3000). <b>N</b> is the number of vertexes and <b>M</b> is the number of edges. Then <b>M</b> lines describing edges follow, each of them contains two integers u, v representing an edge connecting u and v.</p>

<p>Then an integer <b>K</b>, representing the number of nodes whose mark is known. The next <b>K</b> lines contain 2 integers u and p each, meaning that node u has a mark p. It¡¯s guaranteed that nodes won¡¯t duplicate in this part.</p>

<h3>Output</h3>
<p>For each testcase you should print <b>N</b> lines integer the output. The <b>K</b>th line contains an integer number representing the mark of node <b>K</b>. If there are several solutions, you have to output the one which minimize the sum of marks. If there are several solutions, just output any of them.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
3 2
1 2
2 3
2
1 5
3 100

<b>Output:</b>
5
4
100 
</pre>