<p>Consider a table with 2 rows and 2N columns (a total of 4N cells). Each cell of the first row is coloured by one of the colours A, B, C, D such that there are no two adjacent cells of the same colour. You have to colour the second row using colours A, B, C, D such that:</p>

<ul>
  <li>There are exactly N cells of each colour (A, B, C and D) in the table.</li>
  <li>There are no two adjacent cells of the same colour. (Adjacent cells share a vertical or a horizontal side.)</li>
</ul>
<p>It is guaranteed that the solution, not necessarily unique, will always exist.</p>

<h3>Input</h3>
<p>[a natural number N ¡Ü 50000]</p>
<p>[a string of 2N letters from the set {A, B, C, D}, representing the first row of the table]</p>

<h3>Output</h3>
<p>[a string of 2N letters from the set {A, B, C, D}, representing the second row of the table]</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
CB

<strong>Output:</strong>
AD</pre>

<pre><strong>Input:</strong>
2
ABAD

<strong>Output:</strong>
BCDC</pre>