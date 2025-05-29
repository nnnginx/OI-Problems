<p>
You are initially given an empty array of Size <b>N</b> (&lt;=100000). (i.e. each element is 0).
</p>
<p>Given 2 &lt;= <b>R</b> &lt;=10<sup>9</sup>.
</p>
<p>Now you are given 3 types of query:</p>
<ol>
  <li><tt>"0 St i1 i2"</tt>: means add (St, St*R , St*R^2 ,....) GP from i1 to i2 respectively. (Means add the GP with start term St and common ratio R in the series begining from i1 and ending at i2.) </li>
  <li><tt>"1 i j"</tt>: means find the sum of values of the array from index <b>i</b> to index <b>j</b> with modulo 1000000007.</li>
  <li><tt>"2 i"</tt>: resets the <b>i</b>-th index array to 0.</li>
</ol>

<h3>Constraints</h3>
<p>
Queries &lt;=90000<br>
1 &lt;= St &lt;= 10<sup>9</sup>
</p>

<h3>Input</h3>
<p>First Line contains <b>N</b> <b>R</b> <b>Q</b>.<br>
Then Follows <b>Q</b> lines, each line can be of any 3 types described above.</p>

<h3>Output</h3>
<p>Output only second type of Query.</p>

<h3>Example</h3>
<pre><strong>Input:</strong><br>2 2 3<br>0 2 1 2<br>1 1 2<br>1 2 2<br><strong><br>Output:<br></strong>6<br>4</pre>

<p><a href="../INTRO/">Click here to see my set of problems at Spoj.</a></p>