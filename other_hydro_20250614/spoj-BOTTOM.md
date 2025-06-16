<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

<p>
We will use the following (standard) definitions from graph theory.
Let $V$ be a nonempty and finite set, its elements being called vertices (or nodes).
Let $E$ be a subset of the Cartesian product $V \times V$, its elements being called edges.
Then $G = (V, E)$ is called a directed graph.
</p>

<p>
Let $n$ be a positive integer, and let $p = (e_1, \ldots, e_n)$ be a sequence of length $n$ of edges $e_i \in E$ such that $e_i = (v_i, v_{i+1})$ for a sequence of vertices ($v_1, \ldots, v_{n+1}$).
Then $p$ is called a path from vertex $v_1$ to vertex $v_{n+1}$ in $G$ and we say that $v_{n+1}$ is reachable from $v_1$, writing $(v_1 \to v_{n+1})$.
</p>

<p>
Here are some new definitions.
A node $v$ in a graph $G = (V, E)$ is called a sink, if for every node $w$ in $G$ that is reachable from $v$, $v$ is also reachable from $w$.
The bottom of a graph is the subset of all nodes that are sinks, i.e., 
$\mathrm{bottom}(G) = \{v \in V \mid \forall w \in V : (v \to w) \Rightarrow (w \to v) \}$.
You have to calculate the bottom of certain graphs.
</p>

<h3>Input Specification</h3>
<p>
The input contains several test cases, each of which corresponds to a directed graph $G$.
Each test case starts with an integer number $v$, denoting the number of vertices of $G = (V, E)$, where the vertices will be identified by the integer numbers in the set $V = \{1, \ldots, v\}$.
You may assume that $1 \le v \le 5000$.
That is followed by a non-negative integer $e$ and, thereafter, $e$ pairs of vertex identifiers $v_1, w_1, \ldots, v_e, w_e$ with the meaning that $(v_i, w_i) \in E$.
There are no edges other than specified by these pairs. The last test case is followed by a zero.
</p>

<h3>Output Specification</h3>
<p>
For each test case output the bottom of the specified graph on a single line.
To this end, print the numbers of all nodes that are sinks in sorted order separated by a single space character.
If the bottom is empty, print an empty line.
</p>

<h3>Sample Input</h3>
<pre>3 3
1 3 2 3 3 1
2 1
1 2
0</pre>

<h3>Sample Output</h3>
<pre>1 3
2
</pre>