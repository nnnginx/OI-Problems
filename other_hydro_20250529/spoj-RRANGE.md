<p>There are N contiguous cells numbered from 1 to N. Initially, each cell contains a 0 in it. A sub-contiguous group of cells can be updated this way:</p>
<p>1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A range [i,j] is defined such that i &lt; j</p>
<p>2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The cell numbered i is added 1; the cell numbered i + 1 is added 2, and so on until the cell numbered j is reached and added j �C i + 1</p>
<p>For example, if N = 7 and the updates [3, 6] and [4,7] were performed, this is what would happen.</p>
<p>Initially: {0,0,0,0,0,0,0}</p>
<p>Update [3,6]: {0,0,1,2,3,4,0}</p>
<p>Update [4,7]: {0,0,1,3,5,7,4}</p>
<p>&nbsp;</p>
<p>After performing some update operations, it would be amazing to answer questions like the following:</p>
<p>1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A range [u,v] is defined such that u &lt; v</p>
<p>2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The answer is the sum of every cell in the range [u,v] (both u and v are included) modulus 10,000</p>
<p>&nbsp;</p>
<p>Given N and U updates ranges. You have to write a program capable of answering Q questions.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains three integers: N (1 &lt;= N &lt;= 1,000,000,000), U and Q (1 &lt;= U, Q &lt;= 1,000), representing the number of cells, the number of update operations, and the number of questions respectively.</p>
<p>&nbsp;</p>
<p>Each of the following U lines contains two integers i and j (1 &lt;= i &lt; j &lt;= N) separated by a single space indicating an update operation.</p>
<p>Each of the following Q lines contains two integers u and v (1 &lt;= u &lt; v &lt;= N) separated by a single space indicating a question.</p>
<h3>Output</h3>
<p>For each question [u,v] you must print the sum of all contiguous cells starting at u and ending at v modulus 10,000.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 2 2
3 6
4 7
4 6
1 7

<strong>Output:</strong>
15
20</pre>