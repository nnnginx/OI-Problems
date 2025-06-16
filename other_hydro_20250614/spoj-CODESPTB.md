<p>Insertion Sort is a classical sorting technique. One variant of insertion sort works as follows when sorting an array a[1..N] in non-descending order:</p>
<pre>for i &lt;- 2 to N
&nbsp; &nbsp; j &lt;- i
&nbsp; &nbsp; while j &gt; 1 and a[j] &lt; a[j - 1]
&nbsp;  &nbsp; &nbsp; &nbsp;swap a[j] and a[j - 1]
 &nbsp; &nbsp; &nbsp; &nbsp;j &lt;- j - 1</pre>

<p>
The pseudocode is simple to follow. In the ith step, element a[i] is inserted in the sorted sequence a[1..i - 1]. This is done by moving a[i] backward by swapping it with the previous element until it ends up in it's right position.
</p>
<p>
As you probably already know, the algorithm can be really slow. To study this more, you want to find out the number of times the swap operation is performed when sorting an array.
</p>

<h3>Input</h3>
<p>The first line contains the number of test cases T. T test cases follow. The first line for each case contains N, the number of elements to be sorted. The next line contains N integers a[1],a[2]...,a[N].</p>

<h3>Output</h3>
<p>Output T lines, containing the required answer for each test case.</p>

<h3>Constraints</h3>
<p>
1 &lt;= T &lt;= 5<br>
1 &lt;= N &lt;= 100000<br>
1 &lt;= a[i] &lt;= 1000000
</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
5
1 1 1 2 2
5
2 1 3 1 2

<strong>Sample Output:</strong>
0
4</pre>