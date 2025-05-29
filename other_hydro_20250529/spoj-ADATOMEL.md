<p>As you might already know, Ada the Ladybug is a farmer. She grows a tomel  <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. Tomel indeed is a very specific tree. Its growing process starts with one root node with a fruit of random flavor. Whenever a next branch grows, it begins to grow from a random node which is already grown up. No growing starts until the branch is fully grown. As a branch fully grows up, a node with fruit with random flavor appears at the end of the branch.</p>
<p>As you surely haven't heard word random for a long time, Ada chooses three random paths and wants to find the number of distinct flavors which grow on the union of these three paths.</p>
<p><strong>NOTE:</strong> Every random mentioned above is really meant to be random with equal probability for each possible values.</p>
<h3>Input</h3>
<p>The first line of input will contain three integers <strong>N, K, Q</strong>: <strong> 1     ¡Ü N, Q ¡Ü  3*10<sup>5</sup>, 1 ¡Ü K ¡Ü 1000</strong>, the number of nodes of tomel tree, the universe of flavors and the number of Ada's questions.</p>
<p>The next line will contain <strong>N-1</strong> integers <strong>0 ¡Ü P<sub>i</sub> &lt;     i</strong> is the parent of <strong>i<sup>th</sup></strong> node (here <strong>i</strong> goes from <strong>1</strong> to <strong>N-1</strong>).</p>
<p>The next line will contain <strong>N</strong> integers <strong>1 ¡Ü F<sub>i</sub> ¡Ü K </strong>, the flavor of each fruit.</p>
<p>The next <strong>Q</strong> lines will contain six integers <strong>0 ¡Ü B, E, X, Y, L,     R&lt; N</strong>, where the pairs of beginings/ends of the paths are: (<strong>B,     E</strong>), (<strong>X, Y</strong>),  (<strong>L, R</strong>)</p>
<h3>Output</h3>
<p>For each query output the number of distinct flavors which are on the three paths.</p>
<h3>Example Input</h3>
<pre>5 2 5
0 0 0 2
1 1 1 1 2
3 2 3 1 1 4
1 0 2 4 2 3
2 1 4 3 1 0
1 3 3 0 3 1
4 2 0 3 4 1
</pre>
<h3>Example Output</h3>
<pre>2
2
2
1
2
</pre>
<h3>Example Input</h3>
<pre>7 3 7
0 0 0 1 2 3
1 3 2 2 2 1 1
3 2 3 6 3 5
0 2 6 0 4 2
3 6 3 0 2 0
2 0 4 0 2 0
1 5 5 3 2 6
1 2 0 5 0 6
0 4 5 3 2 0
</pre>
<h3>Example Output</h3>
<pre>2
3
2
3
3
3
3
</pre>
<h3>Example Input</h3>
<pre>8 5 7
0 1 0 1 3 0 3
1 1 4 2 3 1 3 1
1 4 2 3 2 4
3 1 4 2 3 6
6 0 0 7 0 6
3 4 2 1 3 4
5 1 0 1 2 1
5 2 4 5 7 6
2 5 1 6 7 2
</pre>
<h3>Example Output</h3>
<pre>4
4
3
4
3
4
4
</pre>
<h3>Example Input</h3>
<pre>12 6 10
0 1 0 2 0 4 4 5 6 6 5
5 4 1 5 3 5 3 5 4 6 4 6
3 9 5 3 5 7
10 8 10 11 6 0
11 6 8 11 3 9
9 2 6 4 8 5
6 5 10 0 2 5
9 11 2 3 2 9
2 3 1 6 10 7
5 2 3 1 9 3
3 4 6 3 6 4
3 8 2 5 0 8
</pre>
<h3>Example Output</h3>
<pre>5
5
5
5
4
5
4
5
4
3
</pre>
<h3>Example Input</h3>
<pre>20 10 22
0 1 2 0 4 5 3 6 8 2 7 2 9 8 13 2 16 10 16
6 7 3 10 7 2 10 6 7 3 6 1 1 3 9 9 8 2 9 3
4 13 5 0 17 7
0 2 8 6 8 13
9 19 12 14 5 13
12 14 9 19 5 18
6 4 9 12 2 16
0 1 11 14 14 0
11 4 17 5 1 13
7 16 1 7 8 15
7 1 14 12 8 16
9 8 18 1 4 18
14 8 4 2 2 12
4 16 3 5 10 19
1 6 7 16 11 12
11 0 5 18 12 8
14 17 0 18 3 19
10 12 5 6 4 10
18 19 14 3 15 9
3 9 13 19 1 18
0 5 3 18 1 16
9 19 12 1 13 7
0 2 7 13 16 19
0 11 3 13 12 4
</pre>
<h3>Example Output</h3>
<pre>6
4
8
8
7
7
7
6
8
4
5
6
7
7
7
6
7
7
7
7
6
6
</pre>