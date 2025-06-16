<p>A number of cities are connected by a network of highways. Each highway is bidirectional and
connects two cities, with a given travel time. What is the shortest time to get from a given city to
another given city?

</p><h3>Input</h3>
<p>The first line of input contains the number of test cases.<br><br>
Each test case starts with a line containing the number of cities n (2 ¡Ü n ¡Ü 100000), the number
of highways m (1 ¡Ü m ¡Ü 100000), the starting city and the ending city. Cities are numbered from
1 to n.<br><br>
Then m lines follow, each describing one highway. The description consists of the two distinct city
numbers and the time in minutes to travel along the highway. The time will be between 1 and
1000.<br>


</p><h3>Output</h3>
<p>For each test case output a single line containing the minimum time it takes to get from the start
to the destination. If no connection exists, output <tt>NONE</tt>.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4 2 1 4
1 2 5
3 4 5
4 4 1 4
1 2 5
2 3 5
3 4 5
4 2 6

<b>Output:</b>
NONE
11</pre>