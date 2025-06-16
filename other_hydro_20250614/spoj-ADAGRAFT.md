<p>As you might already know, Ada the Ladybug is a farmer. She grows a big fruit <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a> (with root in 0). There is a fruit on every node of the tree. Ada is competing in grafting competition and this is her masterpiece. The most valuable tree wins the competition. The value of tree is product of values of each node. The value of a node is the number of distinct fruit kinds in its subtree.</p>
<p>Can you find the value of Ada's tree? Since this number might be pretty big, output it modulo <strong>10<sup>9</sup>+7</strong></p>
<h3>Input</h3>
<p>The first and line will contain <strong> 1 ¡Ü N ¡Ü 4*10<sup>5</sup></strong>.</p>
<p>The next line will contain <strong>N-1</strong> integers <strong>0 ¡Ü p<sub>i</sub> &lt;     i</strong>, the parent of i<sup>th</sup> node.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0 ¡Ü F<sub>i</sub> ¡Ü     10<sup>9</sup></strong>, the fruit growing on i<sup>th</sup> node.</p>
<h3>Output</h3>
<p>Print a single integer - the value of tree modulo <strong>1000000007</strong>.</p>
<h3>Example Input</h3>
<pre>5
0 0 1 1
1 1 1 2 2
</pre>
<h3>Example Output</h3>
<pre>4
</pre>
<h3>Example Input</h3>
<pre>4
0 1 2
6 7 2 3
</pre>
<h3>Example Output</h3>
<pre>24
</pre>
<h3>Example Input</h3>
<pre>11
0 1 1 1 3 5 2 7 5 4
494052753 959648710 959648710 959648710 494052753 959648710 959648710 959648710 959648710 494052753 959648710
</pre>
<h3>Example Output</h3>
<pre>32
</pre>