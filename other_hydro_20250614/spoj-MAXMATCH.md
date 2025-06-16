<p>You're given a string <strong>s</strong> consisting of letters 'a', 'b' and 'c'.</p>
<p>The matching function m<strong><sub>s</sub></strong>( i ) is defined as the number of matching characters of <strong>s</strong> and its i-shift. In other words, m<strong><sub>s</sub></strong>( i ) is the number of characters that are matched when you align the 0-th character of <strong>s</strong> with the i-th character of its copy.</p>
<p>You are asked to compute the maximum of m<strong><sub>s</sub></strong>( i ) for all i ( 1 &lt;= i &lt;= |<strong>s</strong>| ). To make it a bit harder, you should also output all the optimal i's in increasing order.</p>
<h3>Input</h3>
<p>The first and only line of input contains the string <strong>s</strong>. 2 &lt;= |<strong>s</strong>| &lt;= 10<sup>5</sup>.</p>
<h3>Output</h3>
<p>The first line of output contains the maximal m<strong><sub>s</sub></strong>( i ) over all i.</p>
<p>The second line of output contains all the i's for which m<sub><strong>s</strong></sub>( i ) reaches maximum.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
caccacaa

<strong>Output:</strong>
4<br>3<br><br><strong>Explanation:<br><br></strong><pre><span style="font-family: courier new,courier;">cac<strong>cac</strong>a<strong>a</strong><br>   <strong>cac</strong>c<strong>a</strong>caa<br><br><br></span> The bold characters indicate the ones that match when shift = 3.<br><br></pre>
</pre>