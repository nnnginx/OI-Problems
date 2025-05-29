<p>In a galaxy far, far away, the fastest method of transportation is using hypertubes. Each hypertube directly connects K stations with each other. What is the minimum number of stations that we need to pass through in order to get from station 1 to station N?</p>
<h3>Input</h3>
<p>The first line of input contains three positive integers: N (1 ¡Ü&nbsp;N ¡Ü&nbsp;100 000), the number of stations, K (1 ¡Ü&nbsp;K ¡Ü&nbsp;1 000), the number of stations that any single hypertube directly interconnects, and M (1 ¡Ü&nbsp;M ¡Ü&nbsp;1 000), the number of hypertubes.</p>
<p>Each of the following M lines contains the description of a single hypertube: K positive integers, the labels of stations connected to that hypertube.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the required minimum number of stations. If it isn't possible to travel from station 1 to station N, output -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9 3 5
1 2 3
1 4 5
3 6 7
5 6 7
6 8 9

<strong>Output:</strong>
4
</pre>
<pre><strong>Input:</strong>
15 8 4
11 12 8 14 13 6 10 7
1 5 8 12 13 6 2 4
10 15 4 5 9 8 14 12
11 12 14 3 5 6 1 13

<strong>Output:</strong>
3
</pre>
<p>Clarification of the first example: It is possible to travel from station 1 to station 9 using only four stations in the following ways: 1-3-6-9, or 1-5-6-9.</p>