<p>Your task is simple. A knight is placed on the top left corner of a chessboard having <strong>2<em>n</em></strong> rows and <strong>2<em>n</em></strong> columns.
<br>
In how many ways can it move such that it ends up at a corner after atmost <strong><em>k</em></strong> moves ?</p>

<img title="knight" src="../../content/francky:knight" alt="knight" width="50%">


<h3>Input</h3>
<p>The first line contains an integer <strong><em>T</em></strong>, the number of test cases.
Each of the next <strong><em>T</em></strong> lines contains 2 integers : <strong><em>n, k</em></strong>.</p>

<h3>Output</h3>
<p>Output <strong><em>T</em></strong> lines, one for each test case, containing the required total number of configurations.<br>
 Since the answer can get very big, output it modulo 1000007.</p>

<h3>Example</h3>
<pre><b>Input:</b>

3
2 1
2 2
3 3

<b>Output:</b>
1
5
7
</pre>

<h3>Constraints</h3>
<pre>1 &lt;= T &lt;= 50
2 &lt;= n &lt;= 24
1 &lt;= k &lt;= 10^9
</pre>


<h3>Information</h3>
<p>
In the input files, there will be two cases for each possible <strong><em>n</em></strong>.<br>
Constraints allows fast languages to get AC under 0.5s (total time for the 5 input files), with non-optimized scholar methods only.
Advanced methods can be slightly faster, and needed to get AC with interpreted languages (without any guaranty for all of them).<br>
It is recommended to solve first the original problem <a href="http://www.spoj.com/problems/TRKNIGHT/">TRKNIGHT</a> in a very fast way. After that, solve this problem could remain a hard task ; it's not just a simple extension.<br>
Good luck and have fun ;-)
</p>
<p>Edit(12/II/2017, compiler update) New TL.</p>