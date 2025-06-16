<p>Please click <a href="http://www.spoj.com/content/john_jones:hangzhou2008.pdf">here</a> to download a PDF version of the contest problems. The problem is problem A in the PDF. Remember that you must use stdin/stdout at SPOJ.</p>

<hr>

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
We say that two graphs are equivalent if and only if a one-to-one correspondence between their nodes can be established and under such a correspondence their edges are exactly the same. Given $A$ and $B$, two undirected simple graphs with the same number of vertexes, you are to find a series of operations with the minimum cost that will make the two graphs equivalent. An operation may be one of the following two types:
</p>

<ul>
  <li>Add an arbitrary edge ($x$, $y$), provided that ($x$, $y$) does not exist before such an operation. Such an operation costs $I_A$ and $I_B$ on two graphs, respectively.</li>
  <li>Delete an existing edge ($x$, $y$), which costs $D_A$ and $D_B$ on two graphs, respectively.</li>
</ul>

<h3>Input</h3>
<p>There are multiple test cases in the input file.</p>
<p>
Each test case starts with three integers, $N$, $M_A$ and $M_B$, ($1 \le N \le 8$, $0 \le M_A, M_B \le \frac{N(N-1)}{2}$), the total number of vertexes, the number of edges in graph $A$, and the number of edges in graph $B$, respectively. Four integers $I_A$, $I_B$, $D_A$, and $D_B$ come next, ($0 \le I_A, I_B, D_A, D_B \le 32767$), representing the costs as stated in the problem description. The next $M_A + M_B$ lines describe the edges in graph $A$ followed by those in graph $B$. Each line consists of exactly two integers, $X$ and $Y$ ($X \ne Y$, $0 \le X, Y &lt; N$).</p>
<p>
Two successive test cases are separated by a blank line. A case with $N = 0$, $M_A = 0$, and $M_B = 0$ indicates the end of the input file, and should not be processed by your program.</p>

<h3>Output</h3>
<p>Please print the minimum cost in the format as illustrated below.</p>

<h3>Example</h3>
<pre><b>Sample Input</b>
1 0 0
1 2 3 7

4 2 3
1 6 5 1
0 1
0 3
0 2
1 2
1 0

0 0 0

<b>Output for the Sample Input</b>
Case #1: 0
Case #2: 1</pre>