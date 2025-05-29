<p>You are given a simple task.</p>

<p>Given a sequence A[i] with N numbers s.t. 1 &lt;= i &lt;= N. You have to perform Q operations on a given set of numbers.</p>

<p><strong>Operations:</strong>
</p><ol>
  <li><code>A V l</code>, Add the value V to element with index l.</li>
  <li><code>R a l r</code>, Replace all the elements of sequence with index i s.t. l &lt;= i &lt;= r with a.</li>
  <li><code>Q l r</code>, Print the Number of elements with index i s.t. l &lt;= i &lt;= r and A[i] is prime number and A[i] &lt;= 10^7.</li>
</ol>
<p><strong>No Number In sequence ever will exceed 10^9.</strong></p>

<h3>Constraints</h3>
<ul>
  <li>1 &lt;= N &lt;= 10^5</li>
  <li>1 &lt;= Q &lt;= 10^5</li>
  <li>V &lt;= 10^3</li>
  <li>A[i] &lt;= 10^8</li>
  <li>a &lt;= 10^7,&nbsp; 1 &lt;=&nbsp;l &lt;= r &lt;=N.</li>
</ul>

<h3>Input</h3>
<p>
First line contains N as Number of sequence elements &amp;&amp; Q as number of operations to be performed. Second line contains Initial N elements of the sequence. After that each of the next Q lines contains one operation to be performed on the sequence.</p>

<h3>Output</h3>
<p>Print each value in newline as stated above.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>5 10
1 2 3 4 5
A 3 1
Q 1 3
R 5 2 4
A 1 1
Q 1 1
Q 1 2
Q 1 4
A 3 5
Q 5 5
Q 1 5</pre>

<h4>Output</h4>
<pre>2
1
2
4
0
4</pre>