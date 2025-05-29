<p>Jimmy lives in a huge kingdom which contains lots of beautiful cities. He also loves traveling very much, and even would like to visit each city in the country. Jaddy, his secretary, is now helping him to plan the routes, however, Jaddy suddenly find that is quite a tough task because it is possible for Jimmy to ask route��s information toward any city. What was worse is that Jaddy has to response for queries about the distance information nearly between any pair of cities due to the undeterminable starting city which Jimmy is living in when he raises a query. Because of the large scale of the whole country, Jaddy feels hopeless to archive such an impossible job, however, in order to gratify his manager, Jaddy is now looking forward to your assistance.</p>
<p>There might be good news about Jaddy��s work: since Jimmy is very lazy and would not like to travel to a destination whose distance between the original city is larger than TWO. That means only one intermediate city among the route is acceptable (Apparently, all the connecting paths between any two cities, if exists, have the same length as ONE). But don��t be fooled: Jimmy also needs to know that how many alternative different routes are available so that he can have more options. In particular two routes were named as different if and only if there is at least one path in the two routes is distinguishable, moreover, if more than one paths exist between a particular pair of cities, they are considered as distinct.</p>
<h3>Input</h3>
<p>Input has multiple test cases. The first line of the input has a single integer indicating the number of test cases, then each test case follows. For each test case, the first line contains two integers <strong>N</strong> and <strong>M</strong> indicating the number of cities and paths in the country. Then <strong>M</strong> lines are following, each line contains a pair of integers <strong>A</strong> and <strong>B</strong>, separated by space, denoting an undirected path between city <strong>A</strong> and city <strong>B</strong>. All the cities are numbered from 1 to <strong>N</strong>.  Then a new line contains a single integer <strong>Q</strong>, which means there are <strong>Q</strong> queries following. Each query contains a couple of integers <strong>A</strong> and <strong>B</strong> which means querying the distance and number of shortest routes between city <strong>A</strong> and <strong>B</strong>, each query occupies a single line separately.</p>
<p>All the test cases are separated by a single blank line.</p>
<p>You can assume that <strong>N</strong>, <strong>Q</strong> &lt;= 100000, <strong>M</strong> &lt;= 200000.</p>
<h3>Output</h3>
<p>For each test case, firstly output a single line contains the case number, then <strong>Q</strong> lines for the response to queries with the same order in the input. For each query, if there exists at least one routes with length no longer than TWO, then output two integer separated by a single space, the former is the distance (shortest) of routes and the later means how many different shortest routes Jimmy can choose; otherwise, output a single line contains ��The pair of cities are not connected or too far away.�� (quotes for clarifying). See the sample data carefully for further details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 7
1 2
2 3
3 4
4 5
2 5
2 4
1 2
4
1 4
1 2
5 3
5 4

2 0
2
1 1
1 2

<strong>Output:</strong>
Case #1:
2 2
1 2
2 2
1 1
Case #2:
0 1
The pair of cities are not connected or too far away.
</pre>
<pre><strong>Warning: large input/output data, be careful with certain languages</strong></pre>