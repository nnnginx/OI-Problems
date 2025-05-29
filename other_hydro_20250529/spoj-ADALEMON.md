<p>As you might already know, Ada the Ladybug is a farmer. She grows a lemon <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. She wants to pick exactly one lemon (which grows on every leaf of the tree). She is wondering how many distinct trees will remain after harvesting exactly one lemon. Tree is different if they are distinct for each permutation of node labels.</p>
<p>Note that a single node is counted as leaf too.
</p><h3>Input</h3>
<p>The first line of input will contain <strong> 1 ¡Ü T ¡Ü     100</strong>, the number of test-cases.</p>
<p>Each of the testcases will contain single integer <strong>N</strong>, the size of tree.</p>
<p>The next <strong>N-1</strong> lines will contain two integers <strong>0 ¡Ü a, b &lt; N, a ¡Ù b</strong>, the edges of tree.</p>
<p>The sum of <strong>N</strong> over all test-cases will not exceed <strong>3000</strong>.</p>
<h3>Output</h3>
<p>For each test-case output the number of distinct trees after harvesting exactly one lemon.</p>
<h3>Example Input</h3>
<pre>5
4
0 1
0 2
0 3
4
0 1
1 3
3 2
6
0 2
1 2
2 3
3 5
3 4
7
1 2
0 1
2 3
2 4
3 5
6 5
9
0 1
1 2
2 3
3 4
4 5
2 6
3 7
4 8
</pre>
<h3>Example Output</h3>
<pre>1
1
1
3
4
</pre>
<h3>Example Input 2</h3>
<pre>1
11
6 1
3 6
4 3
2 3
0 6
5 2
10 4
8 1
7 10
9 0
</pre>
<h3>Example Output 2</h3>
<pre>3
</pre>