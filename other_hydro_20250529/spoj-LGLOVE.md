<p>Bob fell in love with LCM and GCD. So much that he started seeing LCMs and GCDs everywhere.</p>
<p>Betty, his girl friend was jealous and she gave Bob an array A[ ] of integers, which had nothing to do with LCMs or GCDs.</p>
<p>Quickly, naughty Bob evaluated a new array B[ ] containing n integers, such that B[i] is LCM(1,2,3,...,A[i]), A[i]&gt;0. When A[i] is 0, B[i] is also 0.</p>
<p>Angry Betty decided to give m queries to Bob, each being one of the following type:</p>
<p>-   "0 i j p", meaning add 'p' to each element in A[i..j]. -300000&lt;= p &lt;= 300000 , 0&lt;=i&lt;=j&lt;n</p>
<p>-   "1 i j"    , meaning print the LCM of all elements in B[i..j]. 0&lt;=i&lt;=j&lt;n</p>
<p>-   "2 i j"    , meaning print the GCD of all elements in B[i..j].0&lt;=i&lt;=j&lt;n</p>
<h3>Input</h3>
<p>First line contains n(n &lt;= 100000 ) and m( m &lt;= 35000 ).</p>
<p>Second line contains n integers in the original array A[ ] .</p>
<p>Next m lines contain one of the above said queries.</p>
<p>It is guaranteed that A[i] after any number of updates will satisfy 0&lt;=A[i]&lt;=300000.</p>
<h3>Output</h3>
<p>Output one line for each query of type 1 or 2, modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><pre>5 5<br>4 1 3 6 2<br>1 2 4<br>2 1 3<br>0 0 3 2<br>1 1 2<br>2 2 4<br><br></pre>
<br><br><strong>Output:</strong><br>
<pre>60<br>1<br>60<br>2<br><br></pre>
<br></pre>