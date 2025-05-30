<p>Dystopia consists of N cities. There are one-way roads connecting some pairs of cities. The dysfunctional state has recently seen a lot of protests to overthrow the tyrannical ruler and the government plans to use military patrol vehicles to make sure that the protests are suppressed. Every patrol vehicle is assigned a sequence of cities. If a patrol vehicle is assigned the cities c<sub>1</sub>,c<sub>2</sub>,...c<sub>k</sub> then it starts from the city c<sub>1</sub> and takes the direct one-way road to c<sub>2</sub>, from there it takes the one-way road to c<sub>3</sub> and so on. Finally the vehicle takes the one way road from c<sub>k</sub> to c<sub>1</sub>. This routine is repeated everyday to keep the protestors perpetually under fear.</p>
<p>Now note that:</p>
<ul>
<li> Every city has to appear in exactly one vehicle's patrol sequence exactly once </li>
<li> Every patrol vehicle has to move - so it has to be assigned more than one city </li>
</ul>
<p>&nbsp;</p>
<p>The government does not have any limit on the number of patrol vehicles it can use. However, they want to make sure that the least possible amount of money is spent on the patrol mission and hence they want to minimise the total distance travelled by the patrol vehicles.</p>
<p>Given the road network of Dystopia, find the minimum total distance the patrol vehicles need to move so that all the cities can be patrolled. If it is impossible to organise a nationwide patrol with the given constraints, report the same.</p>
<h3>Input</h3>
<p>First line of the contains T, the number of test cases (T&lt;=10)</p>
<p>This is followed by the descriptions of the T testcases. The first line of the description contains two integers N and R, the number of cities and one way roads respectively (N&lt;=200,R&lt;=10000). The cities are numbered 1,2,3,...N This is followed by R lines, each representing a one way road by 3 integers N<sub>1</sub>, N<sub>2</sub> and D : the start city, the end city and the length of the road respectively ( N<sub>1</sub>!=N<sub>2</sub>, 1&lt;=D&lt;=1000000). You are assured that there is no more than one one way road from any N<sub>1</sub> to N<sub>2</sub></p>
<h3>Output</h3>
<p>For each test case output one line. If the patrol can be done, output the minimum total distance that the patrol vehicles have to travel. Otherwise output Impossible</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3
1 2 1
2 3 1
1 3 1
4 6
1 2 2
2 3 2
3 4 2
4 1 2
1 4 1
3 2 1

<strong>Output:</strong>
Impossible
6
</pre>