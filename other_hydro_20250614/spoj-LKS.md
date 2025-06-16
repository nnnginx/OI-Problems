<p>The&nbsp;<strong><a href="https://en.wikipedia.org/wiki/Knapsack_problem">knapsack problem</a></strong>&nbsp;or&nbsp;<strong>rucksack problem</strong>&nbsp;is a problem in&nbsp;<a>combinatorial optimization</a>: Given a set of items, each with a weight and a value, determine the number of each item to include in a collection so that the total weight is less than or equal to a given limit and the total value is as large as possible. It derives its name from the problem faced by someone who is constrained by a fixed-size&nbsp;<a>knapsack</a>&nbsp;and must fill it with the most valuable items.</p>

<p>Just implement 0/1 Knapsack.</p>

<h3>Input</h3>
<p>First line contains two integers K and N, where K in the maximum knapsack size and N is the number of items. N lines follow where i<sup>th</sup> line describes i<sup>th</sup>&nbsp;item in the form v<sub>i</sub> and w<sub>i</sub> where v<sub>i</sub> is the value and w<sub>i</sub> is the weight of i<sup>th</sup> item.</p>

<h3>Output</h3>
<p>Output a single number - maximum value of knapsack. (All operations and the answer are guaranteed to fit in signed 32-bit integer.)</p>
<p><em>Time limit changed to 2s on 02.07.11.</em></p>

<h3>Example</h3>

<pre><strong>Input:</strong>
10 3
7 3
8 8
4 6

<strong>Output:</strong>
11</pre>

<h3>Constraints</h3>
<p>
K &lt;= 2000000<br>
N &lt;= 500<br>
V<sub>i</sub> &lt;= 10^7<br>
W<sub>i</sub> &lt;= 10^7</p>