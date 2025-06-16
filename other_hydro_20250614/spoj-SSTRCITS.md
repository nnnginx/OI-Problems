<p>Unlike Dystopia, the neighbouring nation of Utopia believes in economic development. To improve the economy of the nation, the Utopian government has decided to select some pairs of cities as sister cities and take steps to improve trade relations between each pair.</p>
<p>There are N cities in Utopia, numbered 1 to N. There are two-way roads  connecting some pairs of cities. The total number of roads in Utopia is R. Now the road network in Utopia has been created efficiently so that there is no road that is redundant. That is, there is exactly one way to travel between any pair of cities without using the same road twice. Now when a pair of cities is chosen as sister cities, the government wants to make sure that there is a direct road between them. Also, a given city cannot have more than one sister.</p>
<p>Given the road network of Utopia, find the number of ways of selecting K pairs of sister cities under these constraints. As the answer can be quite large, output it modulo 100000007.</p>
<p>For example, assume that there are 6 cities in Utopia. There are direct roads between the following pairs of cities : (1,2), (2,3), (2,4), (4,5), (4,6). Notice that  there is exactly one way to travel between any pair of cities. If the government wants to select two pairs of sister cities, it can do it in four ways : {(1,2),(4,5)}, {(3,2),(4,5)}, {(1,2),(4,6)}, {(3,2),(4,6)}</p>
<h3>Input</h3>
<p>First line of the input contains T (¡Ü10), the number of test cases. This is followed by the description of the test cases.</p>
<p>The description of each test case begins with a line containing 3 space separated integers N (&lt;400), R (&lt;10000) and K (&lt;400). Following these are R lines, each representing a road in Utopia. The line will contain two different space separated integers N<sub>1</sub> and N<sub>2</sub> implying that there is a two way road between N<sub>1</sub> and N<sub>2</sub>. You are assured that the road network has the property as described in the problem statement.</p>
<h3>Output</h3>
<p>For each test case, output modulo 100000007 the number of ways of selecting K pairs of sister cities satisfying the conditions in the problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 2 1
1 2
2 3
6 5 2
1 2
2 3
2 4
4 5
4 6

<strong>Output:</strong>
2
4
</pre>