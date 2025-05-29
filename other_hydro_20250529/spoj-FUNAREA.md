<p>There is an M x N matrix of integer numbers.&nbsp; Both the rows and columns of the matrix are numbered starting at 0 and ending at M-1 and N-1 respectively.</p>
<p>A funny area is defined by three integers i,j, and r, and it is composed for those cells [x,y] such that |i-x| + |j-y| &lt;= r. As you might have probably guessed&nbsp;<strong>[i,j]</strong> is the center and <strong>r </strong>is<strong> </strong>the radius of the funny area.</p>
<p>In this problem we are interested in finding the sum of every cell inside some given funny areas.</p>
<h3>Input</h3>
<p>The first line contains two integers 1 &lt;= M, N &lt;= 1000 representing the rows and columns of the matrix.</p>
<p>Each of the following M lines contains N integers separated by single spaces. These numbers are non-negative and not greater than 1,000,000,000</p>
<p>The next line contains a number F (1 &lt;= F &lt;= 100,000) which is the number of funny areas.</p>
<p>Each of the following F lines contains three integers <strong>i</strong>,<strong>j</strong>, and <strong>r </strong>representing the center and the radius of a funny area.</p>
<h3>Output</h3>
<p>F lines: for each funny area print a single number -- the sum of all the cells inside of it.</p>
<h3>Example</h3>
<pre><strong><span style="font-size: large;">Input</span></strong>
5 5
1 2 3 4 5
5 4 3 2 1
1 1 1 1 1
2 3 4 3 0
7 8 9 6 5
3
1 0 0
2 2 2
3 1 1
<p>&nbsp;</p>
<strong><span style="font-size: large;">Output</span></strong>
5
36
18
</pre>
<pre><br class="_<img id="></pre>
<p><img src="./22503/file/s6PipME8.png" alt="" width="155" height="300"></p>