<p>As you might already know, Ada the Ladybug is a farmer. She grows a big lemon <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. She wants to pick exactly one lemon (which grows on every leaf of the tree). She is wondering how many distinct trees will remain after harvesting exactly one lemon. Tree is different if they are distinct for each permutation of node labels.</p>
<h3>Input</h3>
<p>The first and only line will contain <strong> 25 ¡Ü N ¡Ü 3*10<sup>5</sup></strong>.</p>
<p>The next <strong>N-1</strong> lines will contain two integers <strong>0 ¡Ü a, b &lt; N, a ¡Ù b</strong>, the edges of tree.</p>
<h3>Output</h3>
<p>For each test-case output the number of distinct trees after harvesting exactly one lemon.</p>
<h3>Example Input</h3>
<pre>25
18 7
16 18
15 18
8 7
1 8
13 15
22 8
14 18
3 18
23 7
10 8
20 1
21 14
19 3
6 3
9 6
11 7
5 15
17 16
12 22
4 10
24 17
0 8
2 19
</pre>
<h3>Example Output</h3>
<pre>7
</pre>
<h3>Example Input</h3>
<pre>25
6 17
2 6
1 2
13 6
7 6
3 17
16 17
12 7
21 2
0 3
9 12
20 6
8 13
22 2
14 21
19 21
18 21
11 6
10 13
24 19
4 16
5 1
23 10
15 20
</pre>
<h3>Example Output</h3>
<pre>10
</pre>