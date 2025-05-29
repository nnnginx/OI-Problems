<p><br>Shree is a very ambitious person and wants to start a new company "RAM COURIER SERVICE" in the country of Thuvax. He plans to open his first office in the Main Street of Thuvax to serve only the people of this street. The Main Street is an inclined road consisting of N buildings spaced out unevenly(building 1 at lowest level and building N at highest level). The distance between adjacent buildings are known to Shree.<br>&nbsp;<br>The delivery costs incurred by him for various deliveries are calculated as follows:<br>&nbsp;<br>To deliver a package of weight 'w' to a building downhill at a distance 'd' from the office, Shree spends w*d*1 units of money. <br>To deliver a package of weight 'w' to a building uphill at a distance 'd' from the office, Shree spends w*d*2 units of money. <br>To deliver a package of non-zero weight to his own building, Shree spends 10 units of money irrespective of the weight of the package.<br>&nbsp;<br>Shree being an astute businessman wants to choose one of these buildings for his new office so that the total delivery cost incurred by him is minimum. <br>Help Shree choose the building for his new office.</p>
<h3>Input</h3>
<p>The first line of the input consists of number of test cases t(1&lt;=t&lt;=20) <br>&nbsp;<br>The first line of each test case consists of a single number N(1&lt;=N&lt;=10^6) which is the number of buildings in the main street. <br>The next line contains N integers representing the weight to be delivered at ith (1&lt;=i&lt;=N) building (0&lt;=w[i]&lt;=100). <br>The last line contains N-1 integers where the ith (1&lt;=i&lt;=N-1) integer represents the distance between i and i+1 th building(1&lt;=d[i]&lt;=100).</p>
<h3>Output</h3>
<p>Output a single line for each test case containing two integers separated by a space. <br>The first integer is the minimum delivery cost and the next integer is the building number where the office should be placed in order to incur that cost. &nbsp;<br>If more than one building has the same minimum cost, print the building labelled with the smallest number.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 <br>5 <br>1 2 3 4 5 <br>1 1 1 1

<strong>Output:</strong>
30 4
</pre>