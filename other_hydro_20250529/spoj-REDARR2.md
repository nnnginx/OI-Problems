<p>Given an array of size n, you need to reduce the array. In one step, remove any two elements from the array and add their sum instead. Continue addition and removal until no further reduction possible. Output the minimum cost of reduction possible for the given array.&nbsp;</p>
<h3>Input</h3>
<p>First line contains a positive integer T representing number of testcases.</p>
<p>Next line contains a number n denoting the size of array.</p>
<p>Next line contains N space separated positive integers (A[i])</p>
<p>1 ¡Ü T ¡Ü 50</p>
<p>1 ¡Ü n ¡Ü 10<sup>6</sup></p>
<p>1 ¡Ü A[i] ¡Ü 10<sup>6</sup></p>
<h3>Output</h3>
<p>Output minimum cost of reduction.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>4<br>1 6 3 20<br>3<br>2 2 2</pre>
<pre><strong>Output:</strong><br>44<br>10</pre>
<pre><strong>Explanation:</strong><br>Example 1:<br>Remove {1,3} and insert 1+3=4, array becomes [4 6 20], cost=1+3=4<br>Next remove {4,6} and insert 4+6=10, array becomes [10 20], cost=4+6=10 and overall cost=4+10=14<br>Next remove {10,20} and insert 10+20=30, array becomes [30], cost=10+20=30 and overall cost=14+30=44<br>Array cannot be reduced further, hence reduction cost is 44. This sequence of reduciton also gives the minimum possible cost. You will see all other sequences give greater or equal cost.<br><br>Example 2:<br>Remove {2,2} and insert 2+2=4, array becomes [4 2 ], cost=2+2=4<br>Next remove {4,2} and insert 4+2=6, array becomes [6], cost=4+2=6 and overall cost=4+6=10<br>Array cannot be reduced further, hence reduction cost is 10.</pre>