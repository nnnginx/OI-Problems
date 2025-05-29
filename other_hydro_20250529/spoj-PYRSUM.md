<!-- 		@page { margin: 2cm } 		PRE.cjk { font-family: "Droid Sans Fallback", monospace } 		P { margin-bottom: 0.21cm } 		H3 { margin-bottom: 0.21cm } 		H3.cjk { font-family: "Droid Sans Fallback" } 		H3.ctl { font-family: "Lohit Hindi" } -->
<p style="text-align: center;">This is an easier version of <a href="../PYRSUM2">PYRSUM2</a></p>
<p>Tommy is stacking square blocks in columns labelled from 1 to 1000000 (10<sup>6</sup>). Since it can be quite boring writing out the locations of every block he instead specifies a set of 2D pyramids that when built on top of each other will make the shape he wants. Pyramids always have height H=(W+1)/2 and take up N=H<sup>2</sup> blocks so it is quite easy for him to work out how many blocks he will need in total from this description.</p>
<p>What is not so easy is working out how many blocks he will need to build in the space that occurs in the range between two columns (inclusive!). Given a set of instructions consisting of either</p>
<ul>
<li>��build [centre] [w]�� (build another pyramid, width [w] with its midpoint at [centre]) or</li>
<li>��count [left] [right]�� (count the number of blocks added so far within the range of these columns inclusive)</li>
</ul>
<p>you must try to answer the queries as quickly as possible.</p>
<h3>Input</h3>
<p>First line: (1&lt;=T&lt;=20), the number of test cases.</p>
<p>Within each test case:</p>
<ol>
<li>(1&lt;=N&lt;=1000), the number of operations to perform.</li>
<li>N lines, each containing one operation (as detailed above).</li>
</ol>
<h3>Output</h3>
<p>Answer each count query on its own line, putting an additional blank line after each test case.</p>
<p><strong>Please use 64-bit counters as the result may overflow a 32-bit container!</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: andale mono,courier,monospace,times;">4
3
build 5 3
build 6 5
count 4 7
2
build 200 99
count 151 151
4
build 2 1
count 1 1
count 2 2
count 1 2
6
build 5000 3999
count 1 10000
build 2 1
build 3 1
count 2 2
count 2 3
</span>
<strong>Output:</strong>
<span style="font-family: andale mono,courier,monospace,times;">12

1

0
1
1

4000000
1
2</span>

<strong>Visualisation of first test case:</strong>
<span style="font-family: andale mono,courier,monospace,times;">----BB---
----BB---
---BABB--
---AAABB-
   ^  ^</span></pre>