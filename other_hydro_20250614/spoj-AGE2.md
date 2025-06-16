<p>This is the hard version of problem <a href="../SC1">SC1</a>.</p>
<p>"Age of Empires" is a famous real-time strategy game. Resource is one of the most important consideration when playing this game. In this game, there are four different types of resources: food, wood, stone and gold.</p>
<p>The Villager is a common civilian unit for almost every game. They are the backbone of all civilizations. The Villagers are arguably the most important units in the game because they are able to collect all the resources. Each villager could gather A1 units of food, or B1 units of wood, or C1 units of stone, or D1 units of gold. Note that the villager can not split one second into smaller pieces to gather different types of resource. For example, a single villager can not gather A1/2 units of food and B1/2 units of wood for a single second. Moreover, all kinds of recourse are gathered exactly the end of that second. Nevertheless, different villagers could gather different types of resources at a time.</p>
<p>You can also train more villagers to speed up the process of gathering. To train a villager, you must spend X units of food at the beginning of a second, and a new villager will able to work after T seconds. Please note that at the beginning of the second you start to train a villager, you must have not less than X units of food. All villagers are trained at the Town Center but unfortunately there is only one Town Center, so your can only train one villager at a time.</p>
<p>You have N villagers at the beginning of the game with initially no food, wood, stone or gold at all. You are interested in the fastest way to gather enough resources, more precisely, at least A2 units of food and B2 units of wood and C2 units of stone and D2 units of gold.</p>
<h3>Input</h3>
<p>Each test case consists of three lines. The first line contains four integers A1, B1, C1 and D1 (1 &lt;= A1, B1, C1, D1 &lt;= 10^18), indicating the amount of resource a villager can gather for each type in a second. The second line also contains four integers A2, B2, C2 and D2 (0 &lt;= A2, B2, C2, D2 &lt;= 10^18), indicating the amount of resource required. The third line contains three integers N, X and T (1 &lt;= N,X,T &lt;= 10^5), indicating that you have N villager at the beginning of the game, and it will spend X units of food and T seconds to train each new villager.</p>
<p>All integers are sepearted by single spaces.</p>
<p>Process until EOF is reached.</p>
<h3>Output</h3>
<p>For each test case, output a integer - the minimum time to gain enough resources. See the example for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 1 1 1
1 1 1 1
4 1 1
1 1 1 1
2 2 2 2
1 1 1
1 1 1 1
10 10 10 10
1 1 25

<strong>Output:</strong>
Case 1: 1
Case 2: 5
Case 3: 34
</pre>