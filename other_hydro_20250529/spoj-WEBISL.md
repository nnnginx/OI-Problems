<p>For a given set of web pages, we want to find largest subsets such that from every page in a subset you can follow links to any other page in the same subset.</p>
<h3>Input</h3>
<p>On the first line, there are two numbers, number of the pages N, and total number of links M. Pages are numbered from 0 up to N-1. On lines 2 up to M+1, there are two numbers per line. The first is the source page and the second is the target page of a link.</p>
<h3>Output</h3>
<p>On N lines there is a component ID for every single page. The componet ID is the smallest page index on the component.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 3<br>0 1<br>1 0<br>1 2<br><br><strong>Output:</strong>
0<br>0<br>2
</pre>