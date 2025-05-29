<p>You've been invited to the "I-Love-Kd-trees'' annual con, but first, you have to show them that you really know about great data structures, so they give you an easy task! <br><br>You are given a list of<strong> N </strong>numbers and <strong>Q</strong> queries, each query consist of three integers: <em><strong>k</strong>,</em> <strong><em>i</em> </strong>and<strong> <em>l</em></strong> ;let <strong>d</strong> be the <strong>k-th</strong> smallest element until the index <strong>i</strong> (i.e. if the first i+1 elements were sorted in non-descending way, <strong>d </strong>would be the element at index <strong>k - 1</strong> ). Then, the answer to each query is the index of the <strong>l-th</strong> occurrence of <strong>d </strong>in the array. If there's no such index, the answer is <strong>-1.</strong> You have to consider that all indexes are counted starting with <strong>0</strong>.</p>
<h3>Input</h3>
<p>Input consists of one test case.</p>
<p>The first line contains two integers, <strong>N</strong> ( 1 ¡Ü&nbsp; N&nbsp; ¡Ü&nbsp; 10<sup>5</sup>) and <strong>Q</strong> (1 ¡Ü Q&nbsp; ¡Ü 10<sup>5</sup>).</p>
<p>The next line contains <strong>N</strong> possibly distinct integers <strong>a<sub>i</sub></strong> ( -10<sup>9</sup>&nbsp; ¡Ü a<sub>i</sub> ¡Ü 10<sup>9</sup>).</p>
<p><br>Then <strong>Q</strong> lines follow, each of those contains three integers <em><strong>k</strong></em>, <em><strong>i</strong></em> and <em><strong>l</strong></em>. (0 &lt; k ¡Ü&nbsp;i &lt; N, 1 ¡Ü l&nbsp; ¡Ü N).</p>
<h3>Output</h3>
<p><br>For each query (in the same order as the input) output a single line with the answer to that query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><br>10 6<br>2 6 7 1 8 1 2 3 2 6<br>2 4 2<br>2 6 3<br>1 4 1<br>1 4 2<br>3 4 2<br>3 3 2<br>
<strong>Output:</strong>
<br>6<br>-1<br>3<br>5<br>9<br>9<br><br><strong>Explanation of the first query:</strong> <br><br>The elements until index 4 are [2,6,7,1,8] so the 2nd smallest element is 2, and your asked for the index of it's 2nd ocurrency, so the answer is 6.</pre>