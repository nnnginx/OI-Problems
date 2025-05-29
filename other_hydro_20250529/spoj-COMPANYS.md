<p>In China, there are two companies which offer the internet service for the people from all cities: China Telecom and China Unicom. They both are planning to build cables between cities. The government wants to connect all the cities in minimum costs of course. So the minister of finance Mr. B wants to choose some of the cable plans from the two companies and calculate the minimum cost needed to connect all the cities. Mr. B knows that there are <strong>N</strong>-1 cables should be built in order to connect all <strong>N</strong> cities of China. For some political reason, Mr. B should choose <strong>K</strong> cables from the China Telecom and the rest <strong>N</strong>-1-<strong>K</strong> cables from the China Unicom. Your job is to help Mr. B determine which cables should be built and the minimum cost to build them. You may assume that the solution always exists.</p>
<h3>Input</h3>
<p>Each test case starts with a line containing the number of cities <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 50,000), number of cable plans <strong>M</strong> (<strong>N</strong>-1 &lt;= <strong>M</strong> &lt;= 100,000) and the number of required cables from China Telecom <strong>K</strong> (0 &lt;= <strong>K</strong> &lt;= <strong>N</strong>-1).  This is followed by <strong>M</strong> lines, each containing four integers <strong>a</strong>, <strong>b</strong>, <strong>c</strong>, <strong>x</strong> (0 &lt;= <strong>a</strong>, <strong>b</strong> &lt;= N-1, <strong>a</strong> != <strong>b</strong>, 1 &lt;= <strong>c</strong> &lt;= 100, <strong>x</strong>=[0,1]) indicating the pair of cities this cable will connect, the cost to build this cable and the company this cable plan belongs to. <strong>x</strong>=0 denotes this cable plan belongs to China Telecom and <strong>x</strong>=1 denotes this cable plan is from China Unicom.</p>
<h3>Output</h3>
<p>For each test case, display the case number and the minimum cost of the cable building plan.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2 1
0 1 1 1
0 1 2 0
2 2 0
0 1 1 1
0 1 2 0

<strong>Output:</strong>
Case 1: 2
Case 2: 1
</pre>
<p><strong>Explanation</strong></p>
<p>In the first case, there are two cable plans between the only two cities, one from China Telecom and one from China Unicom. Mr. B needs to choose the one from China Telecom to satisfy the problem requirement even the cost is higher.</p>
<p>In the second case, Mr. B must choose the cable from China Unicom, which leads the answer to 1.</p>