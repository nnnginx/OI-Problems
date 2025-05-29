<p>Ada the Ladybug is currently on a trip on apple <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. There are many apples on the tree connected with branches. Each apple is inhabited by either Psylloideas or by Woolly Apple Aphids. Psylloideas and Aphids doesn't like each other, so it is strictly prohibited to walk from apple of Psylloideas to apple of aphids (and vice versa). Ada has some questions, whether it is possible to go from node <strong>I</strong> to node <strong>J</strong>.</p>
<p>Anyway note, that as Aphids and Psyllodeas doesn't like each other, they sometime conquer an apple of the others. Also note, that it is a real apple tree (not some bush) so no apple is connected with more than 50 other apples.</p>
<h3>Input</h3>
<p>The first line contains <strong>1 ¡Ü N, Q ¡Ü 3*10<sup>5</sup> </strong>, number apples on tree and number for queries.</p>
<p>The next line contains <strong>N</strong> characters (either 0 or 1), indicating whether <strong>i</strong><sup>th</sup> apple belongs to Psyllodeas or to Aphids.</p>
<p>Next <strong>N-1</strong> lines contains two numbers, the branches (edges) of apple tree (<strong>0 ¡Ü I, J &lt; N</strong>, <strong>I ¡Ù J</strong>).</p>
<p>Each of following <strong>Q</strong> lines contains one of following types of queries:</p>
<p><strong> 0 I</strong>, <strong>0 ¡Ü I &lt; N</strong>, meaning that ownership of <strong>I</strong><sup>th</sup> apple has changed.</p>
<p><strong> 1 I J</strong>, <strong>0 ¡Ü I, J &lt; N</strong>, question, whether it is possible to go from <strong>I</strong><sup>th</sup> to <strong>J</strong><sup>th</sup> apple.</p>
<h3>Output</h3>
<p>For each query of second kind (1) print "YES", if it is possible or "NO" if it is impossible!</p>
<h3>Example Input</h3>
<pre>8 11
00111100
0 1
1 7
1 2
2 3
2 6
2 4
4 5
1 1 2
1 0 7
1 6 5
1 2 3
1 6 7
0 2
1 1 2
1 0 7
1 6 5
1 2 3
1 6 7
</pre>
<h3>Example Output</h3>
<pre>NO
YES
NO
YES
NO
YES
YES
NO
NO
YES
</pre>