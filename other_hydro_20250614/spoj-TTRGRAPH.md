<p align="justify">Today we continue examine topology of the ancient country GRAPH. It was said that any four cities form a <strong><a href="https://en.wikipedia.org/wiki/Tetrahedron">tetrahedron</a></strong> (or 4-vertex <a href="https://en.wikipedia.org/wiki/Clique_(graph_theory)">clique</a>) if from every city of the tetrahedron there is a road to another tetrahedron city. In the picture below is an example of tetrahedron.</p>
<p align="justify"><em>Theoretical note: all test cases are <a href="https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93R%C3%A9nyi_model">Erdős–Rényi</a> connected low density graphs.</em></p>
<p><img title="TTRGRAPH" src="../../content/julkas:TTRGRAPH.png" alt="TTRGRAPH" width="100%"></p>
<p>Your task is to find the number of tetrahedrons in the country.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p align="justify">The first line of input will contain one integer number <em>4&nbsp;≤&nbsp;N&nbsp;≤&nbsp;900</em>, number of cities in GRAPH. Follow <em>N</em> lines. Each line represents cities (direct neighbors) connected to the city number <em>i</em> (cities numbering is zero based) by one road.</p>
<h3>Output</h3>
<p>Print number of tetrahedrons in the GRAPH.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
1 2 3
0 2 3
0 1 3
0 1 2
</pre>
<pre><strong>Output:</strong>
1
</pre>