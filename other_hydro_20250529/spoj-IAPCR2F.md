<p>In this hot summer AIUB students decided to go on a trip to Cox¡¯s Bazaar sea beach. Every student has some amount of money to spend in this trip. Each student belongs to some group. If student A knows student B, B knows C then A, B and C belong to the same group. In order to utilize the budget properly students hired a travel agency to get an optimal travel plan. They submitted the information about all the student¡¯s money and relations among them. Now the agency wants to figure out the number of groups and the total budget of each group. Total budget of a group is the summation of all the student¡¯s money in that group.</p>
<h3>Input</h3>
<p>The first line contains an integer T (1&lt;=T&lt;=50), denoting the number of test cases.</p>
<p>Each case starts with two integers N M. N (1&lt;=N&lt;=1000), denotes the number of students and M (0&lt;=M&lt;=(N*(N-1)/2)), denotes the number of relationships. In the next line N integers are given. The ith (1&lt;=i&lt;=N) integer a<sub>i</sub> (1&lt;=a<sub>i</sub>&lt;=100) denotes the money ith student has. Next M lines each contains two integers u v, (1&lt;=u,v&lt;=N and u != v) denoting that u knows v and vice versa.</p>
<h3>Output</h3>
<p>For each test case output ¡°Case X: K¡± where X is the case number starting from 1 and K is the number of groups. In the next line output K integers, the total budget of all the groups in ascending order of budget.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5 3
5 7 4 6 8
1 2
1 3
4 5

<strong>Output:</strong>
Case 1: 2
14 16
</pre>