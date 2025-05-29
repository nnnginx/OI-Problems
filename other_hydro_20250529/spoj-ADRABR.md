<p>Adrita, a lady Programmer is at Uttara, at her office. She needs to go home now. But she forgot to take enough money with her. She has limited money, so she can¡¯t afford Uber Ride. She called her friend to give a ride on her bike. But Adrita wants to pay her friend and she wants minimum cost shortest path to reach to her home.</p>
<p>There are several points and there are roads connecting the points. All connecting roads are of length of 1 kilometer. Some roads (like flyover) will charge tolls and the tolls are given. You are to find the shortest path based on minimal cost.</p>
<p>Consider the cost for 1 kilometer is 12 taka for bike ride.</p>
<h3>Input</h3>
<p>In the first line of input, there¡¯s a positive integer k (k &lt;= 50) denoting the number of test cases.</p>
<p>In each test case, the first line contains 4 integers N (1 &lt;= N &lt;= 10^5) denoting the number of  points, R (1&lt;=R&lt;= 10^6) denoting the number of connecting roads, S (1 &lt;= S &lt;= N) denoting the starting point, D (1 &lt;= D &lt;= N) denoting the destination point.</p>
<p>The next R lines contains 3 integers each, U, V (1 &lt;= U, V &lt;= N) and T, (0 &lt;=T &lt;= 10^5) indicating that point U and V are connected with the road which requires toll T taka. All roads are bidirectional and you can assume that the destination point is reachable from the starting point.</p>
<h3>Output</h3>
<p>Print the minimum cost to reach her destination.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>1

6 6 1 6
1 2 0
2 3 0
3 4 1
4 5 2
5 6 0
4 6 12</pre>
<h4>Output</h4>
<pre>61</pre>