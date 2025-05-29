<table class="problems" width="99%"><tbody><tr class="navigation">
<td><a href="/problems/TPERML/polski/">Wersja polska</a></td> 
<td><a href="/problems/TPERML/english/">English version</a></td> 
</tr></tbody></table>



<p>For each index of n element permutation print m subsequent permutations (in separate lines) in lexicographical order starting from the one pointed by index.
Between outputs of subsequent tests there should be an empty line.
Next permutation to the last one is the first one.</p>

<h3>Input</h3>
<p>t [number of tests &lt;= 1000]<br>
n index m [2 &lt;= n &lt;= 100 - number of elements in permutation, 0 &lt;= index &lt; n! - index of the first permutation, 1 &lt;= m &lt;= 100 - how many permutations to print]</p>

<h3>Output</h3>
<p>p1 p2 ... p(n-1) pn [permutations]<br>
p1 p2 ... pn p(n-1)<br>
<br>
p1 p2 ... p(n-1) pn [permutations]<br>
p1 p2 ... pn p(n-1)</p><br>

<h3>Example</h3>

<pre><b>Input:</b>
12
2 1 1
3 3 3
4 16 3
4 5 9
2 1 1
2 1 1
3 5 1
5 91 7
2 1 1
5 100 7
3 5 1
2 1 1

<b>Output:</b>
2 1

2 3 1
3 1 2
3 2 1

3 4 1 2
3 4 2 1
4 1 2 3

1 4 3 2
2 1 3 4
2 1 4 3
2 3 1 4
2 3 4 1
2 4 1 3
2 4 3 1
3 1 2 4
3 1 4 2

2 1

2 1

3 2 1

4 5 1 3 2
4 5 2 1 3
4 5 2 3 1
4 5 3 1 2
4 5 3 2 1
5 1 2 3 4
5 1 2 4 3

2 1

5 1 4 2 3
5 1 4 3 2
5 2 1 3 4
5 2 1 4 3
5 2 3 1 4
5 2 3 4 1
5 2 4 1 3

3 2 1

2 1
</pre>