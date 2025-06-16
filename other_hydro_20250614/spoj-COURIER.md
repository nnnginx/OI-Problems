<p>
	Byteland is a scarcely populated country, and residents of different cities 
	seldom communicate with each other. There is no regular postal service and 
	throughout most of the year a one-man courier establishment suffices to 
	transport all freight. However, on Christmas Day there is somewhat more work 
	for the courier than usual, and since he can only transport one parcel at a 
	time on his bicycle, he finds himself riding back and forth among the cities of 
	Byteland.
</p>
<p>
	The courier needs to schedule a route which would allow him to leave his home 
	city, perform the individual orders in arbitrary order (i.e. travel to the city 
	of the sender and transport the parcel to the city of the recipient, carrying 
	no more than one parcel at a time), and finally return home. All roads are 
	bi-directional, but not all cities are connected by roads directly; some pairs 
	of cities may be connected by more than one road. Knowing the lengths of all 
	the roads and the errands to be performed, determine the length of the shortest 
	possible cycling route for the courier.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	Each test case begins with a line containing three integers: n m b, denoting 
	the number of cities in Byteland, the number of roads, and the number of 
	the courier's home city, respectively (1&lt;=n&lt;=100,1&lt;=b&lt;=m&lt;=10000). The 
	next m lines contain three integers each, the i-th being u<sub>i</sub> v<sub>i</sub>
	d<sub>i</sub>, which means that cities u<sub>i</sub> and v<sub>i</sub> are 
	connected by a road of length d<sub>i</sub> (1&lt;=u<sub>i</sub>,v<sub>i</sub>&lt;=100, 
	1&lt;=d<sub>i</sub>&lt;= 10000). The following line contains integer z - the 
	number of transport requests the courier has received (1&lt;=z&lt;=5). After that, z 
	lines with the description of the orders follow. Each consists of three 
	integers, the j-th being u<sub>j</sub> v<sub>j</sub> b<sub>j</sub>, which 
	signifies that b<sub>j</sub> parcels should be transported (individually) from 
	city u<sub>j</sub> to city v<sub>j</sub>. The sum of all b<sub>j</sub> does not 
	exceed 12.
</p>
<h3>Output</h3>
<p>
	For each test case output a line with a single integer - the length of the 
	shortest possible bicycle route for the courier.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5 7 2
1 2 7
1 3 5
1 5 2
2 4 10
2 5 1
3 4 3
3 5 4
3
1 4 2
5 3 1
5 1 1

<b><tt>Sample output:</tt></b>
43
</pre>