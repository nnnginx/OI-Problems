<p><span style="white-space: pre;"> Professor Mahammad was sitting in his garden</span>&nbsp;when an apple fell on his head, and in a stroke of brilliant insight, he suddenly came up with <em>K-dominant notation</em>. An array with length <em>L</em> is called <em>K-dominant</em>, if and only if there is at least one element <em>x</em> lying in the array for which <strong>occurence(x) * K &gt;= L</strong>. After analyzing several arrays with this property, professor now, made up a new problem for you. Your task is simple, there are given an array of length N and several queries. For each of the queries, you just need to check whether <em>the subarray [l, r] is k-dominant or not</em>.</p>
<h3>Input</h3>
<p>The first line of the input contains two positive integers <strong>N</strong> and <strong>Q</strong>, the number of elements of the array and the mean, respectively. (<strong>N, Q ¡Ü 200000</strong>).</p>
<p>The following line contains N integers which represent elements of the array.</p>
<p>The following Q lines contains three integers <strong>l</strong>, <strong>r</strong>, and <strong>k</strong>. (<strong>1 ¡Ü l ¡Ü r ¡Ü N</strong>).</p>
<p><strong>All the numbers in the input section are 32-bit positive integers.</strong></p>
<p><strong><span style="font-weight: bold;">Sum of all k's in queries does not exceed 500000.</span></strong></p>
<h3>Output</h3>
<p>For each of the queries, print per line <strong>YES</strong> or <strong>NO</strong> if there is an element lying in the subarray which satisfies the condition in the statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8 3
1 4 2 3 2 2 5 3
2 6 2
1 8 2
1 8 3</pre>
<pre><strong>Output:</strong>
YES
NO
YES</pre>
<p><span style="font-family: arial, helvetica, sans-serif;"><em><strong><span style="font-size: medium;">Note</span></strong></em><span style="font-family: arial, helvetica, sans-serif;">: For the first and third queries x = 2 satisfies the condition</span></span>. And for the second query there is no element for which the condition holds true.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>