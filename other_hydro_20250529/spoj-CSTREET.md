<p>The municipal chronicals of an unbelievable lordly major town in a land far, far away tell the following story:<br> Once upon a time the new crowned king G¨¹nther decided to visit all towns in his kingdom. The people of the unbelievable lordly major town expected that king G¨¹nther would like to see some of the most famous buildings in their town. For the lordly citizens it seemed neccessary that all streets in the town that the king would have to use had to be cobbled with stone. Unfortunately the unbelievable lordly major town had not much money at that time as they used most of their savings to erect the highest cathedral the world had ever seen.<br> Roumours were afloat that the real reason for their thriftiness was not that the town treasury was empty but that many people believed that king G¨¹nther came to the throne by deceiving his father king Erwin and that in his youth he made a pact with the devil. But anyway, the citizens of the unbelievable lordly major town decided to pave only as much streets as were absolutely necessary to reach every major building. <br> Can you help the citizens of the unbelievable lordly major town to find out which streets should be paved?<br>It might be usefull to know that all major buildings are either at the end of a street or at an intersection. In addition to that you can assume that all buildings are connected by the given streets.</p>
<h3>Input</h3>
<p>t [number of testcases (1 &lt;= t &lt;= 100)]<br> p [price to pave one furlong of street (positive integer)]<br> n [number of main buildings in the town (1 &lt;= n &lt;= 1000)]<br> m [number of streets in the town (1 &lt;= m &lt;= 300000)]<br> a b c [street from building a to building b with length c (lengths are given in furlong and the buildings are numbered from 1 to n)]</p>
<h3>Output</h3>
<p>For each testcase output the price of the cheapest possibility to reach all main buildings in the city on paved streets.  You can assume that the result will be smaller than 2^32.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
5
7
1 2 1
2 3 2
2 4 6
5 2 1
5 1 3
4 5 2
3 4 3

<strong>Output:</strong>
12
</pre>