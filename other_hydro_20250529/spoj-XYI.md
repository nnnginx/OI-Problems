<pre><span style="font-family: verdana, geneva;"><br><span style="white-space: normal;"><p>You are quite new to Bioinformatics studies. While working in the lab you have met Professor Shakil, who is a bit crazy. You know that there are twenty-two chromosomes and there is the X chromosome and the Y chromosome.</p>
<p>Now Professor Shakil is very determined that there are mutants hiding among us (After watching the new Wolverine movie he went nuts). And he is very positive about a new type of chromosome, which is the I chromosome.</p>
<p>As the Professor is very excited and not suitable for lab work, he will give you a chromosome each time. You have to determine which type it is (X, Y, I or NotValid).</p>
<p>Chromosomes can be viewed as a set of nodes and edges. Look at the images for details. The dotted line represents that there can be an arbitrary number of nodes and edges in these directions (they have to represent a straight line, though).</p><p><img title="XIY" src="../../../content/faiyaz26:xyi.png" alt="XIY" width="550" height="592"></p><p>&nbsp;</p><h4>Input</h4>
<p>In the first line, you will be given the number of test cases T, where T&lt;=200. Then the test cases will follow. Each test case will have two integers at the beginning, N and M. Here N is the number of nodes and M is the number of edges, where 4&lt;=N&lt;=500 and 3&lt;=M&lt;=(N*N-1)/2. Then M lines will follow, each consisting of two integers, U and V, which specifies that there is an edge between node U and node V. It is guaranteed that and given graph will be connected and there will be at most one edge between two nodes.</p>
<p>&nbsp;</p>
<h4>Output</h4>
<p>You have to output the correct chromosome each test case represents, or NotValid if the test case doesn¡¯t represent the three given chromosomes. You have to print ¡°Case T: Z¡±, (without the braces) for each test case, where T is the test case number and Z is the correct chromosome or ¡°NotValid¡±. Please look at the sample I/O for details.</p><span style="font-size: small;"><table style="background-color: #f6f9e0;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td style="font-size: 13px;" width="319" valign="top">
<p style="text-align: justify;"><strong>Sample Input</strong></p>
</td>
<td style="font-size: 13px;" width="319" valign="top">
<p style="text-align: justify;"><strong>Output for Sample Input</strong></p>
</td>
</tr>
<tr>
<td style="font-size: 13px;" width="319" valign="top">
<p style="text-align: justify;">2</p><p style="text-align: justify;">4 4</p><p style="text-align: justify;">1 2</p><p style="text-align: justify;">2 3</p><p style="text-align: justify;">3 4</p><p style="text-align: justify;">4 1</p><p style="text-align: justify;"><span style="font-size: 10px;">4 3</span></p><p style="text-align: justify;">1 2</p><p style="text-align: justify;">2 3</p><p style="text-align: justify;">2 4</p><p style="text-align: justify;">&nbsp;</p>
</td>
<td style="font-size: 13px;" width="319" valign="top">
<p style="text-align: justify;">Case 1: NotValid</p><p style="text-align: justify;">Case 2: Y</p>

</td>
</tr>
</tbody>
</table></span></span></span></pre>
<pre><span style="font-size: x-small;">Problem Setter: Nafis Ahmed</span></pre>
<pre><span style="font-size: x-small;">Special Thanks: Nafis Sadique</span></pre>