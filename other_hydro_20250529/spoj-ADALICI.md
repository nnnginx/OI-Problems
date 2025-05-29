<p>As you might already know, Ada the Ladybug is a farmer. She grows lychee tree. Unlike a cherry tree, lychee tree really forms a tree (obviously a rooted tree - in node <strong>0</strong>). The lychee fruits grow in bunches (there are (usualy) multiple lychee fruits in each node).</p>
<p>Ada will give you many queries, for harvesting lychees, consisting of 3 numbers: <strong>index of node U</strong>, <strong>I<sup>th</sup> ancestor</strong>, <strong>L new lychees</strong>, meaning, that she wants to harvest lychees of <strong>I<sup>th</sup> ancestor</strong> of node <strong>U</strong>. Afterward <strong>L</strong> new lychee fruits will grow on the node.</p>
<p>She wants you to sum all those harvest-values and output the sum. Value of harvest can be counted as <strong>X*W</strong>, where <strong>X</strong> is number of node where you'll harvest and <strong>W</strong> is the number of lychees in it.</p>
<p>Also note that input's format won't be easy (as usual). You will be given description of the tree and <strong>x<sub>0</sub>, a, b</strong>. The next term could be counted as <strong>x<sub>i</sub>=(a*x<sub>i-1</sub>+b)%MOD</strong>, where % means modulo and <strong>MOD</strong> is equal to <strong>10^9+7</strong> (<strong>1000000007</strong>)</p>
<p>Firstly, you can set the number of lychees on each node: The number of lychee fruits on node <strong>i</strong> is equal to <strong>x<sub>i</sub>%100003</strong> (<strong>10<sup>5</sup>+3</strong>). Afterward there will be <strong>Q</strong> queries, giving you <strong>U, I, L</strong> (denoting <strong>XT</strong> as next <strong>x<sub>i</sub></strong>), <strong>U=XT%N</strong>, <strong>I=XT%(D[U]+1)</strong> (where <strong>D</strong> indicates DEPTH - root has depth 0), <strong>L=XT%100003</strong> [priority of XT is from left to right].</p>
<p><strong>NOTE:</strong> Parent of every node will always have lesser ID than the node itself (since the lychees far away from root are much more juicy).</p>
<h3>Input</h3>
<p>The first line contains five integers <strong> N, Q, x<sub>i</sub>, a, b:  1 ¡Ü     N ¡Ü 2*10<sup>5</sup>, 1 ¡Ü Q ¡Ü 4*10<sup>7</sup>, 0 ¡Ü a, b,     x<sub>0</sub> &lt; 1000000007</strong></p>
<p>The next <strong>N-1</strong> lines contains two integers <strong>0 ¡Ü a &lt; b &lt; N</strong>, the branch connecting two nodes.</p>
<h3>Output</h3>
<p>Print a single line - the number sum of values over all queries.</p>
<h3>Example Input</h3>
<pre>5 3 1 1 1
0 1
1 2
0 3
2 4
</pre>
<h3>Example Output</h3>
<pre>13
</pre>
<h3>Additional Information</h3>
<pre>#LYCHEES: 1 2 3 4 5
QUERY 1: 1 1 8
QUERY 2: 4 2 11
QUERY 3: 2 1 14
</pre>
<h3>Example Input 2</h3>
<pre>5 5 2 3 4
0 1
1 2
2 3
2 4
</pre>
<h3>Example Output 2</h3>
<pre>113299
</pre>
<h3>Additional Information 2</h3>
<pre>#LYCHEES: 2 10 34 106 322
QUERY 1: 0 0 8746
QUERY 2: 2 1 36188
QUERY 3: 1 0 77101
QUERY 4: 4 2 81719
QUERY 5: 0 0 26368
</pre>
<h3>Example Input 3</h3>
<pre>10 100 666 561 14159
0 1
0 2
1 3
1 4
2 5
2 6
3 7
3 8
4 9
</pre>
<h3>Example Output 3</h3>
<pre>9060951
</pre>
<h3>Example Input 4</h3>
<pre>20 10000 30355495 415740782 580959825
0 1
1 2
2 3
3 4
3 5
0 6
6 7
7 8
8 9
3 10
1 11
3 12
11 13
3 14
3 15
4 16
16 17
8 18
17 19
</pre>
<h3>Example Output 4</h3>
<pre>1939449924
</pre>