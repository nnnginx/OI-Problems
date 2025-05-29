<p>The Slovak national railroad company has recently built new tracks. They want to update their railroad map according to these changes. But they want the map to be as simple as possible. So they decided to remove from the map all the stations that have exactly two other direct connections to other stations (i.e., a single railroad passing through the station).</p>

<h3>Problem specification</h3>

<p>You will be given the complete map of Slovak railroads. It consists of railway stations numbered from 1 to N, and railroad segments between some pairs of these stations. For each railroad segment we are given its length.</p>

<p>Your task is to remove all such stations that are directly connected with exactly two other stations, and output the new map. The new map must contain correct distances between the remaining stations.</p>

<h3>Input specification</h3>

<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line. 

</p><p>Each test case begins with a line with two integers N(1&lt;= N &lt;=2000) and M(1&lt;= M &lt;=3000). The number N denotes the number of stations and M is the number of railroad segments. M lines follow, each with 3 integers a, b, and c (1 &lt;= a,b &lt;= N) specifying that there is a railroad segment of length c connecting stations a and b. 

</p><p>You can assume that in each test case there is a path between every two stations, and there is at most one railroad between any pair of cities directly. Also, there will always be at least 2 stations that are not directly connected to exactly two other stations. </p>

<h3>Output specification</h3>

<p>For each test case, the output shall consist of multiple lines. The first line shall contain a positive integer K �C the number of railroads on the simplified map. Each of the next K lines shall contain three integers a, b (a must be no more than b), and c stating that there is a railroad of length c between stations a and b on the simplified map. 
</p><p>The railroads should be listed in lexicographic order, i.e. the railroad with less a should be listed first,if two railroads have the same a, then the one with less b should be listed first. If two railroad have the same a and b, the one with less c should be listed first.
</p><p>Print a blank line between outputs for different test cases.</p>

<h3>Example</h3>
<pre><b>input:</b>
2

3 2
1 2 1
2 3 1

4 4
1 2 1
2 3 2
3 4 3
4 2 1

<b>output:</b>
1
1 3 2

2
1 2 1
2 2 6
</pre>
<h3>Hint</h3>
<p>In the first case we removed station 2 beacuse it had exactly 2 direct connections. 

</p><p>In the second case we removed stations 3 and 4. We see that there is now a railroad from station 2 back to itself.</p>

<p>For all the test cases, <b>int</b> in C/C++/Java or <b>longint</b> in Pascal is enough.</p>