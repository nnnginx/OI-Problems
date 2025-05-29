<p>Petya is the mayor of a city named Mayapur. In the morning, everybody likes to drink hot tea in bed, and the citizens need milk to take with their tea. For this purpose, they should be able to reach at least some milkman in the city. There are m bi-directional roads in the city but all of them are currently unrepaired, hence not in a state of use. <br>Petya cares about his city a lot and intends to repair some of these roads, so that every citizen is connected to at least one milkman. For repairing each road he needs to pay a cost. He would like to minimize the cost of this project. Note that a milkman does not need to go to some other milkman for milk as he can take milk from himsaelf.&nbsp;</p>
<p>Help Petya in finding out the minimum cost needed to repair the roads in the given way. If it is not possible for a citizen to connect to any of the milkmen, output "impossible" (without quotes).</p>
<h3>Input</h3>
<p>The first line contains T: the number of test cases. (1 &lt;= T &lt;= 100)</p>
<p>For each test case, the first line contains two space-seperated numbers n, m: n is the number of citizens in Mayapur and m denotes the number of unrepaired roads  (1 &lt;= n &lt;= 10^5, 1 &lt;= m &lt;= min (n * (n - 1) / 2, 2 * 10^5)).</p>
<p>The next line contains n space-separated integers, which are either 0 or 1, denoting for successive citizens whether they are a milkman or not.</p>
<p>Then, for each of the next m lines, each line contains three space-seperated integers u, v and c, denoting that there exists a unrepaired road between u and v such that the cost of repairing of road is c. (1 &lt;= u, v &lt;= n and u != v, 1 &lt;= c &lt;= 10^9.)&nbsp;</p>
<h3>Output</h3>
<p>For each test case output the cost as required.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5 7
0 1 0 1 0
1 2 11
1 3 1
1 5 17
2 3 1
3 5 18
4 5 3
2 4 5
<strong>Output:</strong>
5
</pre>