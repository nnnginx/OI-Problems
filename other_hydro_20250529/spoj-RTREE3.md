<p>Roger was able to solve his problem based on tree last time, only because of your help. He has been doing good and is learning and&nbsp;practicing various problems on trees (as he likes solving problems on connected undirected acyclic graphs). This time he is stuck with&nbsp;a harder problem and has spent almost a week trying to solve this problem, with no efficient solution till now. But, he has you as his&nbsp;friend and he knows that only you can help him with your excellent programming skills.</p>
<p>You will be given an input in the form of a growing tree. ie; Initially you have a tree consisting only of vertex <strong>1</strong>.&nbsp;At each step, the tree will grow. So next, vertex <strong>u</strong> will be connected to vertex <strong>1</strong>, then vertex <strong>v</strong> will be connected to either&nbsp;vertex <strong>1</strong> or vertex <strong>u</strong>, and so on till you get a tree consisting of <strong>'N'</strong> vertex.&nbsp;However, at any instant, while adding the vertexes you will be given a vertex <strong>'x'</strong> (which is already present in the tree grown so far),&nbsp;and you will be asked to print the eccentricity of the given vertex <strong>x.</strong></p>
<p>Let <strong>G</strong> be a graph and <strong>'x'</strong> be a vertex of G.</p>
<p>The eccentricity of the vertex <strong>'x'</strong> is the maximum distance from 'x' to any vertex present in G.</p>
<p>That is, <strong>e (x) = max {d (x, y) : y is in G}.</strong></p>
<p>Of Course vertex <strong>y</strong>, should also be present in the tree, grown so far.</p>
<p>Along with the eccentricity, you should also print the vertex <strong>'y'</strong>.</p>
<p>Please help Roger.</p>
<h3>Input</h3>
<p>The first line contains <strong>'N'</strong> and <strong>'M'</strong>, where N = Number of nodes in the tree and M = Number of Queries.</p>
<p>Next M lines will either have an input of the type <strong>"U x y" </strong>or <strong>"Q x".</strong></p>
<p>For the input of type <strong>"U x y"</strong>, &nbsp;you have to connect the vertex <strong>'y'</strong> to the vertex <strong>'x'</strong>, where vertex<strong> 'x'</strong> is already present in the tree and vertex <strong>'y'</strong> is the new vertex. Obviously, there will be <strong>(N - 1)</strong> inputs of the type <strong>"U x y"</strong>.</p>
<h3>Output</h3>
<p>For each input of the type <strong>"Q x"</strong>, you have to print the eccentricity of vertex <strong>'x'</strong>, followed by the vertex <strong>'y'</strong>.</p>
<p>If there are multiple such <strong>'y'</strong>. Print the <strong>smallest 'y'</strong>.</p>
<h3>Example</h3>
<pre><strong>Sample Input</strong>
5 8
Q 1
U 1 4
Q 1
U 4 2
U 1 5
U 5 3
Q 1
Q 2

<strong>Sample Output</strong>
0 1
1 4
2 2
4 3</pre>
<h3>Explanation</h3>
<p>Initially, the tree has vertex 1.</p>
<p>Q 1 &nbsp; =&gt; Eccentricity of vertex 1 is 0.</p>
<p>U 1 4 =&gt; Connect vertex 4 to vertex 1.</p>
<p>Q 1 &nbsp; =&gt; Eccentricity of vertex 1 is 1.</p>
<p>U 4 2 =&gt; Connect vertex 2 to vertex 4.</p>
<p>U 1 5 =&gt; Connect vertex 5 to vertex 1.</p>
<p>U 5 3 =&gt; Connect vertex 3 to vertex 5.</p>
<p>Q 1 &nbsp; =&gt; Eccentricity of vertex 1 is 2. Vertex 2 and Vertex 3 both are at a distance of 2 from vertex 1. Print the smaller one.</p>
<p>Q 2 &nbsp; =&gt; Eccentricity of vertex 2 is 4.</p>
<h3>CONSTRAINTS</h3>
<p>1 &lt;= N &lt;= 10^5<br> N - 1 &lt;= M &lt;= 2*N<br> 1 &lt;= x, y &lt;= N</p>