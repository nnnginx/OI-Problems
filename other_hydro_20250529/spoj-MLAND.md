<p>
	With every year, the plans for the construction of motorways in Poland are more 
	and more advanced. For some time, it seemed as if the building was actually 
	going to start, so the question of purchasing the land under the roads was of 
	some importance. Only certain cities can be connected by a road directly, 
	provided the farmer owning the land under it agrees to sell out. As a result of 
	the constant swing of moods, the price demanded for the land by each farmer 
	changes in a linear fashion, with possibly different coefficients for every 
	road. It may either increase or decrease (and sometimes even be negative, if 
	the owner anticipates future profit from the proximity of a motorway).
</p>
<p>
	It has been decided that the purchase of land will be made at some moment in 
	between two fixed dates. At that moment, the current prices of land will be 
	frozen, and the least costly configuration of bidirectional roads connecting 
	all cities (directly or indirectly) will be chosen. All the land under the 
	selected roads will subsequently be bought at the frozen price. Since business in the proximity of a motorway does have its advantages, some land owners might actually want their land to be bought and they may offer money into the bargain, consequently making the price of purchase negative.
</p>
<p>
	You act as an intermediary for the purchase and charge a steady commission, 
	proportional to the total sum of purchase. Oddly enough, when signing the contract you missed the clause about the possibility of the price being negative and now you begin to wonder whether you won't end up being charged for your own hard work. Since it is one of your tasks to 
	select the moment of purchase, do so in such a way as to maximise your profit (if this is impossible, at least cut your losses as much as possible).
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line contains two integers n m, denoting the 
	number of cities to be connected and the number of available potential 
	roads,respectively(1&lt;=n&lt;= 120,1&lt;=m&lt;=820). The next line contains 
	two integers t<sub>1</sub> t<sub>2</sub>, which stand for the earliest possible 
	and latest possible moments of purchase (-10000&lt;=t<sub>1</sub>&lt;=t<sub>2</sub>&lt;=10000). 
	Each of the following m lines contains four integers, the i-th being: u<sub>i</sub>
	v<sub>i</sub> a<sub>i</sub> b<sub>i</sub>, which means that the i-th road 
	connects city u<sub>i</sub> with city v<sub>i</sub>, and the purchase of the 
	land under it costs b<sub>i</sub>+j*a<sub>i</sub> units of 
	currency at moment j (e.g. at moment 0 the land costs b<sub>i</sub>
	units). Please note that these integers are chosen from the following ranges: 
	0&lt;=u<sub>i</sub>,v<sub>i</sub>&lt;=n-1, -32000&lt;=a<sub>i</sub>,b<sub>i</sub>&lt;=32000.
</p>
<h3>Output</h3>
<p>
	For each test case output a line with two floating point numbers, accurate to 
	three digits after the decimal point. The first represents the moment of 
	transaction you ought to choose, the second - the total value of the 
	transaction at that moment. If more than one moment fulfills the conditions of the problem, choose the earliest.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2
5 6
0 5
1 0 -6 -4
2 0 3 -3
3 0 1 5
3 1 -2 -3
4 1 -3 -2
4 3 -2 -3
5 7
-20 20
1 0 1 2
2 1 -7 4
3 1 -9 0
3 2 4 9
4 1 0 -2
4 2 2 3
4 3 6 -5

<b><tt>Sample output:</tt></b>
0.000 -13.000
0.111 -1.000
</pre>