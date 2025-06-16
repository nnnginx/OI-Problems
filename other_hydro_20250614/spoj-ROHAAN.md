<p>Kingdom of Rohan is under attack! There are N vital army stations. King will decide what army should be guarding what station, to get the best strategic advantage against Sauron attacks. All armies are already in some stations, but not necessarily the stations required by the king. As a result armies will have to be moved. Distances between any pair of stations are known. They are not necessarily symmetrical, because road from station A to B could be different than road from B to A. When a army moves, it doesn't have to take a direct road and instead can choose to cross other stations, if that results in a shorter path.</p>

<p>Given the distances between stations and king's relocation orders, find the minimum total travel distance for all the armies.</p>

<h3>Input</h3>

<p>First line contains an integer <b>T</b>, number of test cases. Then the description of <b>T</b> test cases follow. Each test case starts with an integer <b>N</b>, which is the total number of army stations. Next <b>N</b> lines have <b>N</b> integers each, description of distances. <b>b</b>'th integer on line <b>a</b> is the distance from station <b>a</b> to station <b>b</b>. Description of kings orders follows. In a first line, a single integer <b>R</b>, number of orders. Next <b>R</b> lines will contain two integers <b>s</b> and <b>d</b> each, describing an order to move an army from station <b>s</b> to <b>d</b>.</p>

<p><b>Constrains:</b></p>
<p>1 &lt;= T &lt;= 50</p>
<p>1 &lt;= N, R &lt;= 50</p>
<p>1 &lt;= distance &lt;= 10^6</p>
<p>1 &lt;= s, d &lt;= N</p>

<h3>Output</h3>

<p>Print a single line for each test case. A string "Case #t: " without quotes, where <b>t</b> is the number of test case, starting from 1. Following the string, you must print the total distance armies must travel during relocation.</p>

<p>0 &lt;= total distance &lt;= 10^7</p>

<h3>Example</h3>

<pre><b><u>Input:</u></b>
1
3
0 1 1
1 0 1
1 9 0
2
2 1
3 2

<b><u>Output:</u></b>
Case #1: 3
</pre>