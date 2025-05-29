<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/TPCPPLAR/en/">English</a></td>
<td width="50%"><a href="/problems/TPCPPLAR/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given a directed graph G , N vertices and M arcs.&nbsp;</p>
<p>A node X called "acessible" to Y if there is a path from X to Y</p>
<p>A node X called "popular" if every node Y in V fulfill one of two conditions :</p>
<p>1. X is acessible to Y</p>
<p>2. Y is acessible to X</p>
<p>The Problem : &nbsp;Given graph G, count the number of popular node.</p>
<p>&nbsp;</p>
<p>Input</p>
<p>- The first line contain N and M, the number of nodes and arcs (1 &lt;= N &lt;= 150000; 1 &lt;= M &lt;= 300000)</p>
<p>- M next lines, each line contains x and y, there is a arcs connect from x to y. &nbsp;</p>
<p>&nbsp;</p>
<p>Output</p>
<p>- First line print number of popular nodes.</p>
<p>- Second line print populars node in increasing order.&nbsp;</p>
<p>Example</p>
<p>Input:</p>
<p>5 4</p>
<p>1 2</p>
<p>3 2</p>
<p>2 4</p>
<p>4 5</p>
<p>Output:</p>
<p>3</p>
<p>2 4 5</p>
<p> </p>