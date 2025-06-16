<p>Ada the Ladybug grows a mulberry <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a> (which is rooted at node 0). At the beginning, it has a mulberry fruit of distinct size growing on every node. As the time flows, new mulberry fruits appear on each node (additionally - meaning the previous mulberry fruit still remains on given node) - while keeping the condition of distinct sizes.</p>
<p>Ada observes every single fruit and for each new fruit she is asking you to tell her the number of lesser fruits in the subtree of given node.</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>1 ¡Ü N, Q ¡Ü 2*10<sup>5</sup> </strong>, size of mulberry tree.</p>
<p>The next line contains <strong>N</strong> integers: <strong>0 ¡Ü A<sub>i</sub> ¡Ü     10<sup>6</sup></strong>, the size of mulberry fruit in each node.</p>
<p>Each of the next <strong>N-1</strong> lines contains two integers <strong>0 ¡Ü a, b &lt; N</strong>, meaning the branch (edge) between given nodes.</p>
<p>Each of the next <strong>Q</strong> lines contains two integers <strong>a S</strong>: <strong>0 ¡Ü     a &lt; N</strong> (the node in which new fruit grows) and <strong>0 ¡Ü S ¡Ü     10<sup>6</sup></strong> (size of the fruit)</p>
<h3>Output</h3>
<p>For each query, print the number of lesser mulberry fruits which grow in subtree of node where new mulberry fruit grew.</p>
<h3>Example Input</h3>
<pre>7 8
10 9 13 17 11 20 18
0 4
0 1
1 2
1 3
2 5
2 6
0 21
0 8
2 15
3 22
1 14
2 19
0 12
1 16
</pre>
<h3>Example Output</h3>
<pre>7
0
1
1
2
3
4
4
</pre>