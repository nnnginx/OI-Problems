<p>The dwellers of the island Abstinence are very fond of alkoholfree beer. Hitherto alkohol-free beer was imported from Poland, but this year one of the cities on Abstinence is going to build a brewery. All the cities of this island lie on the coast and are connected by a highway running around the island along its shore. The investor building the brewery collected information about the demand for beer, i.e. how many tanks of beer are needed daily in each city. He has also a table of distances between cities. The cost of transporting one tank is 1 thaler per mile. A daily cost of transport is the amount of money, which has to be spent on transporting a necessary number of tanks of beer from the brewery to each city. The daily cost depends on the location of the brewery. The investor wants to find a location that minimizes the daily cost.

</p><h3>Task</h3>
<p>Write a program which
</p><ul>
<li> reads the number of cities, distances between them and daily requests for beer,
</li><li> computes the minimal daily cost of transport,
</li><li> writes the result.
</li></ul>

<h3>Input</h3>
<p>There are multiple test cases. Their number is given in the first line of input. In the first line of each test case there is one integer n - the number of cities, 5 &lt;= n &lt;= 10 000. (We assume that cities are numbered along the highway, so that the neighbouring cities have subsequent numbers. Cities 1 and n are neighbours too.) In each of the following n lines there are two non-negative numbers separated by a single space. Numbers zi di written in the line (i+1) are respectively the demand for beer in the city i and the distance (in miles) from city i to the next city on the highway. The entire length of the highway is not greater than 1 000 000 miles. The demand for beer in each city is not greater than 1 000 tanks.

</p><h3>Output</h3>
<p>For each test case your program should write only one line - exactly one integer equal to the minimal daily cost of transport.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
6
1 2
2 3
1 2
5 2
1 10
2 3

<b>Output:</b>
41
</pre>