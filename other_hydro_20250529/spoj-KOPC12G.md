<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="white-space: pre;"> </span>You are given an alphabetical matrix of size NxN .You have to perform two kinds of operations 1) Update and 2) query.The matrix contains only Uppercase English alphabets.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Update operation is to replace a row or &nbsp;column of the matrix with the given string.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Query Operation returns the count of each alphabest in the query region.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The operations are given as</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A) 0 &nbsp;x y str -&gt; Replace &nbsp;y th row with string str if x=0 or update yth column with string str (top to bottom) if (x=1)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">B) 1 &nbsp; x1 y1 x2 y2 -&gt; Count the number of each alphabets in the rectangular region where (x1,y1) is topleft point of the rectangle and (x2,y2) is the bottom right point of the rectangle.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For count operation Print Output;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">where Output=1*number &nbsp;of A's + 2*number of B's + ...... 26*number of Z's;</div>
<p><span style="white-space: pre;"> </span>You are given a matrix of size NxN containing only upper case alphabets .You have to perform two kinds of operations:&nbsp;</p>
<p>Replace operation is to replace a row or column of the matrix with the given string.</p>
<p>Count Operation returns the count of each alphabet in the required region.</p>
<p>The operations are given as</p>
<p><strong>0 x y str </strong>-&gt; Replace &nbsp;y th row with string str, if x=0 or update yth column with string str (top to bottom), if x=1</p>
<p><strong>1 x1 y1 x2 y2</strong> -&gt; Count the number of each alphabets in the rectangular region of the matrix where (x1,y1) is top-left point of the rectangle and (x2,y2) is the bottom-right point of the rectangle.</p>
<p>For every Count operation output the value of (1*number of A's + 2*number of B's + ...... 26*number of Z's).</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of the input file contains T &nbsp;which denotes the number of test cases.</p>
<p>The first line of each test case contains two integers N and q where N denotes size of the matrix and q denotes the number of queries. This is followed by NxN alphabetic matrix. The matrix is followed by q lines of queries, in the above given format.&nbsp;</p>
<p>T&lt;=10</p>
<p>N&lt;=500, Q&lt;=10000</p>
<p>0&lt;=x1&lt;N, 0&lt;=x2&lt;N, 0&lt;=y1&lt;N, 0&lt;=y2&lt;N&nbsp;</p>
<p>x1&lt;=x2, y1&lt;=y2</p>
<p>Warning: Huge I/O</p>
<h3>Output</h3>
<p>Print the output for each query line by line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
4 3
ABCD
ABCD
ABCD
ABCD
1 0 0 3 3 
0 0 2 PQRS
1 0 2 3 3


<strong>Output:</strong>
40
58</pre>