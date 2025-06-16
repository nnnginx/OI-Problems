<p>&nbsp;&nbsp;&nbsp; You are given n numbers. Any two number are called friends if they have some digit common. eg. (11, 12) and (15, 4561) are friends but (33, 556) is not.</p>
<p>&nbsp;&nbsp;&nbsp; Find out no of pairs which are friends.</p>
<p>&nbsp;&nbsp; &nbsp;(Formally speaking Let us assume the n numbers be are stored in array a[]. You have to find out number of i and j pairs such that i &lt; j and a[i] and a[j] are friends.).</p>
<h3>Input</h3>
<p>T : no of test cases (T &gt;= 1 &amp;&amp; T &lt;= 7)&nbsp;<br>For each test case, you will be given two lines, first line will contain n &lt;= 10^6<br>then in next n line each line will contain a single integer representing a[i] (a[i] &gt;= 1 &amp;&amp; a[i] &lt;= 10^18)</p>
<h3>Output</h3>
<p>For every test case print a line <br>containing number of such pairs as mentioned in the problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4</pre>
<pre>2</pre>
<pre>12&nbsp;13</pre>
<pre>3</pre>
<pre>10&nbsp;12&nbsp;24</pre>
<pre>3</pre>
<pre>5&nbsp;6&nbsp;7</pre>
<pre>4</pre>
<pre>10&nbsp;11&nbsp;211&nbsp;3</pre>
<p><strong>Output:</strong> <br>1<br>2<br>0<br>3</p>