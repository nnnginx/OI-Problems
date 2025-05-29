<p>
Segment trees are extremely useful. In particular "Lazy Propagation" (i.e. <a href="http://stackoverflow.com/questions/10832954/data-mapping-and-lazy-propagation-in-segment-tree">see here, for example</a>) allows one to compute sums over a range in O(lg(n)), and update ranges in O(lg(n)) as well. In this problem you will compute something much harder: 
</p>
<p><strong>The sum of squares over a range with range updates of 2 types: </strong></p>
<p><strong>1) increment in a range </strong></p>
<p><strong>2) set all numbers the same in a range.</strong></p>

<h3>Input</h3>
<p>
There will be <strong>T</strong> (<strong>T</strong> &lt;= 25) test cases in the input file. First line of the input contains two positive integers, <strong>N</strong> (<strong>N</strong> &lt;= 100,000) and <strong>Q</strong> (<strong>Q</strong> &lt;= 100,000). The next line contains <strong>N</strong> integers, each at most 1000. Each of the next <strong>Q</strong> lines starts with a number, which indicates the type of operation:
</p>

<p>
2 <strong>st nd</strong> -- return the sum of the squares of the numbers with indices in [<strong>st</strong>, <strong>nd</strong>] {i.e., from <strong>st</strong> to <strong>nd</strong> inclusive} (1 &lt;= <strong>st</strong> &lt;= <strong>nd</strong> &lt;= <strong>N</strong>).
</p>

<p>
1 <strong>st nd x</strong> -- add "x" to all numbers with indices in [<b>st</b>, <b>nd</b>] (1 &lt;= <b>st</b> &lt;= <b>nd</b> &lt;= <b>N</b>, and -1,000 &lt;= <b>x</b> &lt;= 1,000).
</p>

<p>
0 <b>st nd x</b> -- set all numbers with indices in [<b>st</b>, <b>nd</b>] to "<b>x</b>" (1 &lt;= <b>st</b> &lt;= <b>nd</b> &lt;= <b>N</b>, and -1,000 &lt;= <b>x</b> &lt;= 1,000).
</p>

<h3>Output</h3>
<p>
For each test case output the <tt>¡°Case &lt;caseno&gt;:¡±</tt> in the first line and from the second line output the sum of squares for each operation of type 2. Intermediate overflow will not occur with proper use of 64-bit signed integer.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 5
1 2 3 4
2 1 4
0 3 4 1
2 1 4
1 3 4 1
2 1 4
1 1
1
2 1 1

<strong>Output:</strong>
Case 1:
30
7
13
Case 2:
1</pre>