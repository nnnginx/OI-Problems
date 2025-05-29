<p>
You are given a <strong>1-indexed</strong> array <strong>X</strong>, consisting of<strong> N</strong> integers, and a set of <strong>Q</strong> queries. There are two kinds of queries:</p>

<ol>
  <li><strong>0 a b c</strong><br> Here you are required to return the number of elements with indices in <strong>[a,b]</strong><br> greater than or equal to <strong>c</strong></li>
  <li><strong>1 a b</strong><br> Here you are required to change the <strong>a<sup>th</sup></strong> element of array to <strong>b</strong>. </li>
</ol>

<h3>Input Format:</h3>
<p>First line contains <strong>N</strong>, the number of elements in the array <strong>X</strong>. The next line   contains <strong>N</strong> space separated integers representing the elements of <strong>X</strong>. The third   line of input contains a single integer, <strong>Q</strong>, the number of queries. The next <strong>Q</strong> lines of input each contain queries of two kinds as described above. </p>

<h3>Output Format:</h3>
<p><strong>Q </strong>lines with the ith line contains the answer for the <strong>i<sup>th</sup></strong> query </p>

<h3>Constraints:</h3>
<p>1 ¡Ü N ¡Ü 5*10^5<br> 1 ¡Ü Q ¡Ü 10^5<br> 1 ¡Ü X[i] ¡Ü 10^9<br> 1 ¡Ü a ¡Ü b ¡Ü N for query type 0<br> 1 ¡Ü a ¡Ü 10^5, 1 &lt; b ¡Ü 10^9 for query type 1<br> 1 ¡Ü c ¡Ü 10^9<br></p>

<h3>Example</h3>
<pre><b>Sample Input:</b>
5
1 2 3 4 5
3
0 1 5 10
1 2 20
0 1 3 10

<b>Sample Output:</b>
0
1</pre>

<p><strong>Problem Setter: Pulkit Goel and Vidit Gupta</strong></p>