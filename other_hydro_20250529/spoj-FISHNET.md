<p>In a highly modernized fishing village, inhabitants there make a living on fishery. Their major tools, fishing nets, are produced and fixed by computer. After catching fishes each time, together with plenty of fishes, they will bring back the shabby fishing nets, which might be full of leaks. Then they have to inspect those nets. If there exist large leaks, they have to repair them before launching out again.</p>
<p>Obviously, the smaller the leaks in the fishing nets are, the more fishes they will catch. So after coming back, those fishermen will input the information of the fishing nets into the computer to check whether the nets have leaks. The checking principle is very simple: The computer regards each fishing net as a simple graph constructed by nodes and edges. In the graph, if any circle whose length (the number of edges) is larger than 3 must has at least one chord, the computer will output "<tt>Perfect</tt>" indicating that the fishnet has no leaks. Otherwise, "<tt>Imperfect</tt>" will be displayed and the computer will try to repair the net.</p>
<p>&nbsp;</p>
<p><br><strong>Note:</strong>&nbsp;A circle is a closed loop, which starts from one node, passes through other distinct nodes and back to the starting node. A chord is an edge, which connects two different nodes on the circle, but it does not belong to the set of edges on the circle.</p>
<h3>Input</h3>
<p>The input file contains several test cases representing different fishing nets. The last test case in the input file is followed by a line containing&nbsp;<tt>0 0</tt>.</p>
<p>The first line of each test case contains two integers,&nbsp;<span><em>n</em></span>&nbsp;and&nbsp;<span><em>m</em></span>&nbsp;, indicating the number of nodes and edges on the net respectively,&nbsp;<span>1<img src="file://TasT6icn.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>n</em><img src="file://TWyxXDNu.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">1000</span>&nbsp;. It is followed by&nbsp;<span><em>m</em></span>&nbsp;lines accounting for the details of the edges. Each line consists of two integers&nbsp;<span><em>x</em><sub>i</sub></span>&nbsp;and&nbsp;<span><em>y</em><sub>i</sub></span>&nbsp;, indicating there is an edge between node&nbsp;<span><em>x</em><sub>i</sub></span>&nbsp;and node&nbsp;<span><em>y</em><sub>i</sub></span>&nbsp;.</p>
<h3>Output</h3>
<p>For each test case, display its checking results. The word "<tt>Imperfect</tt>" suggests that the corresponding fishing net is leaking, while the word "<tt>Perfect</tt>" stands for a fishing net in good condition.</p>
<p>Follow the output for each net with a blank line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre><pre>4 4
1 2
2 3
3 4
4 1
3 3
1 2
2 3
3 1
0 0</pre>
<strong>Output:</strong></pre>
<pre><pre>Imperfect

Perfect</pre>
</pre>