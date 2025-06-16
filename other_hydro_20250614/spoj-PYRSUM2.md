<p style="text-align: center;">This is a harder version of <a href="../PYRSUM">PYRSUM</a></p>
<p>Tommy is stacking square blocks in columns labelled from 1 to 1000000 (10<sup>6</sup>).  Since it can be quite boring writing out the locations of every block  he instead specifies a set of 2D pyramids that when built on top of each  other will make the shape he wants. Pyramids always have height  H=(W+1)/2 and take up N=H<sup>2</sup> blocks so it is quite easy for him to work out how many blocks he will need in total from this description.</p>
<p>What is not so easy is working out how many blocks he will need to  build in the space that occurs in the range between two columns  (inclusive!). Given a set of instructions consisting of either</p>
<ul>
<li>��build [centre] [w]�� (build another pyramid, width [w] with its midpoint at [centre]) or</li>
<li>��count [left] [right]�� (count the number of blocks added so far within the range of these columns inclusive)</li>
</ul>
<p>you must try to answer the queries as quickly as possible.</p>
<h3>Input</h3>
<p>(1&lt;=N&lt;=200000), the number of operations to perform.</p>
<p>N lines, each containing one operation (as detailed above).</p>
<ol> </ol>
<h3>Output</h3>
<p>Answer each count query on its own line, putting an additional blank line after each test case.</p>
<p><strong>Please use 64-bit counters as the result may overflow a 32-bit container!</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: andale mono,courier,monospace,times;">3
build 5 3
build 6 5
count 4 7
</span>
<strong>Output:</strong>
<span style="font-family: andale mono,courier,monospace,times;">12
</span>
<strong>Visualisation of example test case:</strong>
<span style="font-family: andale mono,courier,monospace,times;">----BB---
----BB---
---BABB--
---AAABB-
   ^  ^</span></pre>