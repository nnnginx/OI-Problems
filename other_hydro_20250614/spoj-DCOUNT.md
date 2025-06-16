<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">Given an integer 'K', construct a set 'S' containing all integers from 1 to 2*K-1 (both inclusive). Construct a graph 'G' with vertices represented by all the K-1 element subsets of 'S'. There is an&nbsp; edge from vertex 'u' to vertex 'v' in 'G', if the corresponding subsets of 'u' and 'v' do not have any element in common. The distance d(u,v) between a vertex 'u' to a vertex 'v' is defined as the shortest path from 'u' to 'v' in 'G'. The diameter of 'G' is defined as the longest distance between any two vertices in 'G'. Output the diameter of the graph and the number of pairs of vertices which have distance equal to the diameter.</span></span></p>
<h3>Input</h3>
<p align="justify"><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">The first line  of input contains a number 't', the number of test cases.</span></span></p>
<p align="justify"><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">Each of the  following 't' lines contains an integer 'K'.</span></span></p>
<h3>Output</h3>
<p><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">For each testcase output two space separated integers, the diameter and the number of pairs. Since the numbers can be huge, output all the numbers modulo 1,000,000,007.</span></span></p>
<h3>Example</h3>
<pre><span style="font-family: arial black,avant garde;"><strong>Input:</strong></span></pre>
<pre><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">2</span></span></p><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">2</span></span></p><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">3</span></span></p></pre>
<pre><span style="font-family: arial black,avant garde;"><strong>Output:</strong></span></pre>
<pre><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">1 6</span></span></p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">2 60</span></span><strong><br></strong></pre>
<pre><span style="font-family: arial black,avant garde;"><strong>Explanation:</strong></span></pre>
<p>
</p><p><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;"><strong>For Case 1:</strong></span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">The graph is a triangle, so&nbsp; the diameter is 1 and the distance between any 2 pairs of different&nbsp; vertices is 1. The 6 pairs are: ({1},{2}), ({2},{1}), ({1},{3}),({3},{1}),&nbsp; ({2},{3}), ({3},{2}).</span></span></p>
<p></p>
<pre><span style="font-family: arial black,avant garde;"><strong><strong>Constraints:</strong></strong></span></pre>
<pre><pre><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">t &lt;= 25</span></span></p><p><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">2 &lt;= K &lt;= 100,000</span></span></p></pre>
</pre>