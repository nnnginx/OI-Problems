<p>We say that a 2-dimensional, rectangular word w of size n¡Ám (imagine it as a board with letter written in the squares) can be tiled with a rectangular pattern p if there are such occurrences of p in w (but not necessarily all of them) that no two of them overlap and each symbol (square) of w is covered by one of them.  Given such word w, find a rectangular pattern p of smallest size (area) which the word w can be tiled with.</p>
<h3>Input</h3>
<p>The first line of input contains a number t (1¡Üt¡Ü100) that indicates the number of test cases to follow. Each test case begins with a line consisting of two positive integers n and m (1¡Ün,m¡Ü1000) indicating dimensions of the board. n lines follow, each of them containing m small letters of the English alphabet (a,b,...,z).</p>
<h3>Output</h3>
<p>For each test case output the smallest possible area of a pattern p that can be used to tile the given board.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
4 3
aaa
aaa
aaa
aaa
4 4
abab
cdcd
abab
cdcd
3 4
aaaa
aaaa
aaab

<strong>Output:</strong>
1
4
12

</pre>