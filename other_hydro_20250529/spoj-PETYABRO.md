<p>Petya lives in a city named Mayapur. As in the morning, everybody likes to drink hot tea in the bed. So the citizens of Mayapur needs milk to produce tea. For this purpose, they want to be able to go to a milkmen using the bi-directoinal roads. There are m roads in the city. Every year these roads become unfit for transportation, hence they have to be repaired each year.</p>
<p>Last Year Petya repaired those roads. as Petya is short in money last year he repaired them such thatwith minimum budget&nbsp;everyone get milk from someone. Since then he received some complaints that some people have to walk for a long distance to get milk so this year Petya want to repair the roads such that everyone can go to their nearest milkmen to get milk. So he has to select some roads to repair such that every citizen is connected to atleast one milkman and that milkman is the nearest one for that citizen. For reparing each road he needs to pay the necessary cost. As he does not want to spend a lot of money in it, He wants to minimize the cost needed in this project. Note that a milkmen does not need to go to some other milkmen for milk as he can take milk from his own home. But Petya was a little bit bored to plan this time so he asked his brother to help him.</p>
<p>Now it is your job to help Petya Brother in finding out minimum cost needed to repair the roads in the above given way. If it is not possible for a citizen to connect to any of the milkmen, output "impossible" (without quotes).</p>
<p>PS: Note that you should print the minimum cost needed such that everyone can go to their nearest milkman.</p>
<h3>Input</h3>
<p>First line contains two space seperated number n, m: number of citizens in Mayapur and m denotes number of unrepaired roads.</p>
<p>Next line contains n space integers either 0 or 1 which indices that citizen is milkmen or not[1 means he is a milkman]. (1 &lt;= n &lt;= 10^5)</p>
<p>Then For each of the next m lines, each line contains three space seperated integers u, v and c, denoting that there exists a unrepaired road between u and v such that cost of repairing of road is c. (1 &lt;= u, v &lt;= n and u != v)</p>
<p>(1 &lt;= m &lt;= min (n * (n - 1) / 2, 2 * 10^5). 1 &lt;= c &lt;= 10^9.)</p>
<h3>Output</h3>
<p>Print the cost if not possible print "impossible".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 7
0 1 0 1 0
1 2 11
1 3 1
1 5 17
2 3 1
3 5 18
4 5 3
2 4 5

<strong>Output:</strong>
5
</pre>
<p>
PS: for python users please make your submission using fastio or u can submit the solution into pypy.
</p>