<p>Mr. White has found a way to maximize the purity of crystals based on certain chemical compounds. He has observed that each compound is made of molecules that are linked together following the structure of a complete binary tree where every level, except possibly the last, is completely filled, and all nodes are as far left as possible. Each node of the tree stores the valence of a molecule and is represented as an integer number. Mr. White uses an electronic microscope that dumps the molecule structure as a stream of integer numbers and would like to have your help on automatically obtaining the total valence of only the leaves of the given tree. For example, the sequence 4-3-2-6-0-3 represents the tree shown in the figure and the total valence of the leaves is 9.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/henu:ucv2013J" alt="Sample Tree" width="181" height="186"></p>
<h3>Input</h3>
<p>The input contains several test cases, each one corresponding to a particular compound. Each test case consists of a single line starting with an integer N (1  &lt;= N&nbsp; &lt;= 1000000), followed by N integer numbers Vi representing the valences of each molecule separated by blank spaces (0 &lt;= Vi &lt;= 100).</p>
<p><br>The end of input is indicated by a test case with N = 0.</p>
<h3>Output</h3>
<p>For each compound output a single line with the sum of the valences of the leaves of the tree.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 4 3 2 6 0 3<br>7 1 1 1 2 1 2 1<br>0

<strong>Output:</strong>
9<br>6<br>&nbsp;</pre>