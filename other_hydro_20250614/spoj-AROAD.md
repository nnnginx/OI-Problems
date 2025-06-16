<h3>Problem</h3>
<p align="justify">
Let's say you are given a set of cities (numbered from 1 to n) and possible bidirectional roads between them. You would like to build cheapest road network that will make getting from the capital (which has number 1) to every other city possible, where the cost of the network is just sum of its roads' costs. Seems easy? Well, it certainly would be too easy and boring, so this time you should satisfy one additional constraint: you must consider only networks in which there are at most d roads outgoing from the capital.
</p>
<h3>Input</h3>
<p align="justify">
First line of input contains number of test cases c (1&lt;=c&lt;=40). Each test case begins with number of cities n, number of possible roads m and maximum degree d (1&lt;=n&lt;=1000, 0&lt;=m&lt;=100000, 0&lt;=d&lt;=100). Then m lines describing roads follow, each of them containing road endpoints x,y and its cost c (1&lt;=x,y&lt;=n, 0&lt;=c&lt;=10000).
</p>
<h3>Output</h3>
<p align="justify">
For each test case output the cost of building cheapest road network or NONE if it is impossible.
</p>
<h3>Example</h3>
<pre>Input:
4
4 5 0
1 2 1
1 3 1
1 4 2
2 3 2
3 4 1000

4 5 1
1 2 1
1 3 1
1 4 2
2 3 2
3 4 1000

4 5 2
1 2 1
1 3 1
1 4 2
2 3 2
3 4 1000

4 5 3
1 2 1
1 3 1
1 4 2
2 3 2
3 4 1000

Output:
NONE
1003
5
4

</pre>