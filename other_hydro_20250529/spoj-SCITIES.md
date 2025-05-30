<p>
Far, far away there is a world known as Selfishland because of the nature of its inhabitants. Hard times have forced the cities of Selfishland to
exchange goods among each other. C1 cities are willing to sell some goods and the other C2 cities are willing to buy some goods (each city can either
sell or buy goods, but not both). There would be no problem if not for the selfishness of the cities. Each selling city will sell its goods to one city
only, and each buying city will buy goods from one city only.


<br><br>Your goal is to connect the selfish cities in such a way that the amount of exchanged goods is maximalized.



</p><h3>Input</h3>
<p>The first line contains a positive integer t&lt;=1000 indicating the number of test cases. Each test case is an instance of the problem defined above. The first line of each test case is a pair of positive integers C1 and C2 (the number of cities wanting to sell their goods C1&lt;=100 and the number of cities wanting to buy goods C2&lt;=100). The lines that follow contain a sequence of (c1,c2,g) trios ending with three zeros. (c1,c2,g) means that the city c1 can offer the city c2 the amount of g&lt;=100 goods.


</p><h3>Output</h3>
<p>
For each test case print the maximal amount of goods exchanged.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
3 2
1 1 10
2 1 19
2 2 11
3 2 1
0 0 0
4 4
1 1 6
1 2 6
2 1 8
2 3 9
2 4 8
3 2 8
4 3 7
0 0 0
3 2
1 1 10
2 1 21
2 2 11
3 2 1
0 0 0

<b>Output:</b>
21
29
22
</pre>