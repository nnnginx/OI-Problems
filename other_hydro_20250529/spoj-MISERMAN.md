<p>Jack is a wise and miser man. Always tries to save his money.</p>
<p>One day, he wants to go from city A to city B.  Between A and B, there are N number of cities(including B and excluding A) and in each city there are M buses numbered from 1 to M. And the fare of each bus is different. Means for all N*M busses, fare (K) may be different or same.  Now Jack has to go from city A to city B following these conditions:</p>
<ol>
  <li>At every city, he has to change the bus.</li>
  <li>And he can switch to only those buses which have number either equal or 1 less or 1 greater to the previous.</li>
</ol>

<p>You are to help Jack to go from A to B by spending the minimum amount of money.</p>
<p>N, M, K &lt;= 100.</p>

<h3>Input</h3>
<p>Line 1:&nbsp;&nbsp; &nbsp;N M<br>Line 2-:&nbsp;&nbsp;&nbsp; NxM Grid</p>
<p>Each row lists the fares the M busses to go form the current city to the next city.</p>

<h3>Output</h3>
<p>Single Line containing the minimum amount of fare that Jack has to give.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5 5
1  3  1  2  6
10 2  5  4  15
10 9  6  7  1
2  7  1  5  3
8  2  6  1  9

<strong>Output:</strong>
10</pre>

<h3>Explanation</h3>
<p>1 -&gt; 4 -&gt; 1 -&gt; 3 -&gt; 1: 10</p>