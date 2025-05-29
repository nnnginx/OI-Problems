<p>You are given a complete undirected graph with <strong>n</strong> nodes numbered from 1 to <strong>n</strong>. You are also given <strong>k</strong> <em>forbidden</em> edges in this graph.</p>
<p>You are asked to find the number of Hamiltonian cycles in this graph that don't use any of the given <strong>k</strong> edges. A Hamiltonian cycle is a cycle that visits each vertex exactly once. A cycle that contains the same <em>edges</em> is only counted once. For example, cycles 1&nbsp;2&nbsp;3&nbsp;4&nbsp;1 and 1&nbsp;4&nbsp;3&nbsp;2&nbsp;1 and 2&nbsp;3&nbsp;4&nbsp;1&nbsp;2 are all the same, but 1&nbsp;3&nbsp;2&nbsp;4&nbsp;1 is different.</p>
<h3>Input</h3>
<p>The first line of input gives the number of cases, <strong>N</strong> (¡Ü 10). <strong>N</strong> test cases follow. The first line of each test case contains two integers, <strong>n</strong> (¡Ü 300) and <strong>k</strong> (¡Ü 15). The next <strong>k</strong> lines contain two integers each, representing the vertices of a  forbidden edge. There will be no self-edges and no repeated edges.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #<strong>X</strong>: <strong>Y</strong>", where <strong>X</strong> is the case number (starting from 1) and <strong>Y</strong> is the number of Hamiltonian cycles that do not include any of those <strong>k</strong> edges. Print your answer modulo 9901.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<code> 2<br> 4 1<br> 1 2<br> 8 4<br> 1 2<br> 2 3<br> 4 5<br> 5 6</code>

<strong>Output:</strong>
<code> Case #1: 1<br> Case #2: 660</code>
</pre>