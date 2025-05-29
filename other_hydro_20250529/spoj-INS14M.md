<p>
In his final interview Digo is given a map of a city containing N junctions connected by roads of length 1. 
There is only one path between any two junctions. Each junction has a unique index between 1 and N(inclusive). 
There are M Civilians in the city. Everyday, each civilian visits a set of junctions.
</p>

<p>
There are military camps built at certain junctions. 
The terrorists are planning to attack the city by targeting some junctions. 
However due to the presence of military camps, 
there is a limit to the size of explosion they can make at any particular junction. 
The intensity of the bomb planted at a junction is equal to the minimum distance from 
any military camp to the targeted junction. 
The damage of all civilians passing through a targeted junction increases by 
the intensity of the bomb dropped at the junction. 
The military camps set up and the terrorist targets are given in the form of the following queries:<br><br>
1 J : Meaning that a new military camp is set up at junction J<br>
2 J : Meaning that the junction J is targeted by terrorists<br>
3 J : Print the total damage done till now to all civilians visiting junction J<br><br>

Initially there is exactly one military camp at junction 1. 
The initial damage of all civilians is given to you.

</p><h3>Input</h3>
<p>First line contains 3 integers N, M, Q. N is the number of junctions, M is the number of civilians and Q is the number of queries to follow.</p>

<p>Next N-1 lines contains 2 integers U and V (denoting that there is a road connecting U and V).</p>

<p>Next M lines contains one integer each. The ith line contains integer a[i] representing the initial damage of the ith civilian. Next M lines contain the description of the junctions visited by the ith civilian (First integer of every line is X, the number of junctions visited by the ith civilian, followed by X integers representing the respective junctions). </p>

<p>Next Q lines give the corresponding queries. Each query can be described by two integers T, J, where T is the type of query (which can be 1 or 2 or 3) and J is the respective junction of the query.
</p>

<h3>Output</h3>

<p>For all the queries of type 3 print an integer answering the query.</p>

<h3>Constraints</h3>
<p>1 &lt;= N &lt;= 50000<br>
1 &lt;= M &lt;= 10000<br>
1 &lt;= Q &lt;= 50000<br>
1 &lt;= X, V, U, J &lt;= N<br>
1 &lt;= a[i] &lt;= 1000<br><br>
Sum of all the junctions crossed by all the civilians is less than 50001<br><br>
Note: The Final answer will fit in 64 bit signed integer.<br><br></p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
3 1 3
1 2
2 3
5
2 2 3
3 3
2 3
3 3

<strong>Sample Output:</strong>
5
7</pre>