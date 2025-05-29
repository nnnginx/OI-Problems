<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Professor Mahammad was busy with working their machine learning project in XYZ University. His team collected many data for the analysis of specific procedures. As the length of individual data objects were quite large, he used a popular hashing technique for getting a unique identifier for each data. Unfortunately, the hashing function generated similar result strings for data. As it is not suitable for the project, he started to think what to do with those strings. Suddenly, he came up with a new idea for a problem for beginners. Now he asks, for the given strings in each query, how many lexicographically smaller or equal strings exist in the input?&nbsp;</p>
<h3>Input</h3>
<p>First line of the input contains two positive integers N and Q, respectively, the number of input strings and the number of queries.</p>
<p>The following N lines represent the strings generated from the procedure.</p>
<p>Finally, the next Q lines contain the query strings which you need to process.</p>
<p>The input section contains strings with only lowercase English letters.</p>
<h3>Output</h3>
<p>For each of the Q lines, you need to output the number of equal or lexicographically smaller strings.</p>
<h4 style="font-size: 10px; white-space: pre;"><em><span style="font-size: small;">Note: The sum of the lengths of the input and query strings does not exceed 200000, seperately.</span></em></h4>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 3
fury
fuzzy
dizzy
future
fuzz
evil
freeze</pre>

<pre><strong>Output:</strong>
3
1
1</pre>