<p>As you probably know there is a new kind of energy called V-energy which is more afordable than electricity, and has some really interesting properties. The Universal Company on V-Energy has just reached your city and is currently planning the location of the distribution centers. You are given a map of the city, the list of the location of the distribution centers, and they need you to report which is the minimum ammount of energy that would reach a building of the city, and how many buildings share that ammount of energy</p>
<p>V-Energy has the following properties:</p>
<p>&nbsp;</p>
<ul>
<li> If a buiding has K units of V-Energy it will consume C units and distribute K - C to every building it is connected to. If K &lt; C the building will consume K units and will not distribute any units of energy</li>
<li> If a building receives V-Energy from different sources it will only consume and distribute the energy with maximum value. For example, if a building receives K = 8 units of energy,and C = 3 it will consume 3 and distribute 5. But, if later the same building receives K = 6 units of energy, it will not consume or distribute this energy since previously it received a larger ammount of energy. If later on the same building receives K = 15 units of energy, it will consume 3 units, and distribute 12 units to its neighbors </li>
</ul>
<p>As you know, your city is a grid, with buildings on every intersection of the streets. Since V-Energy propagates only through streets, the streets map of the city is perfect for your job. Avenues run horizontally while streets run vertically. Note that sometimes a street or avenue can be blocked. The next figure shows a possible view of a city where street 1 is blocked between<br>avenues 1 and 2, and avenue 2 is blocked between streets 0 and 1.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/henu:ucv2013D" alt="Streets and avenues sample" width="428" height="200"></p>
<h3>Input</h3>
<p>The input contains several test cases. Each case starts with a line containing the values K and C (ammount of V-energy each distribution center has and ammount of V-energy each building consumes). (0 &lt;= C,K&nbsp; &lt;= 10000). The next line contains two values N and M denoting the number of avenues and streets on the city (1 &lt;= N,M &lt;= 1000). The following line will have one value B which denotes the number of street and avenues segments that are blocked and cannot distribute V-energy (0 &lt;= B&lt;=  N*M-N-M). The following B lines will have four values T I J1 J2. T indicates the type of the segment, can be either 'A' of 'S' to denote an avenue segment or a street segment. I denotes the street or avenue index (0 &lt;=I &lt; N). If it is an avenue segment then J1, J2 are the indexes of the starting street and ending street where the avenue is blocked. If it is a street segment, J1, J2 are the indexes of the starting and ending avenues where the street is blocked (0 &lt;= J1 &lt; J2 &lt;= M). The next line will have the<br>number D of deposits (0 &lt;=  D &lt;= min(1000,N*M)). The following D lines will have a pair Ai Si indicating that on the intersection of avenue Ai with street Si there will be a distribution center. (0 &lt;= Ai &lt; N, 0 &lt;= Si &lt; M).</p>
<p><br>The end of input is indicated by a test case with K = C = 0.</p>
<h3>Output</h3>
<p>For each test cases you have to print a line containing two numbers Q and P indicating the minimum amount of energy that reaches a building on the city, and the number of building with that amount of energy.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 1<br>2 3<br>0<br>2<br>0 0<br>0 2<br>12 2<br>3 3<br>2<br>A 2 0 1<br>S 1 1 2<br>1<br>2 0<br>0 0

<strong>Output:</strong>
0 1<br>2 1 <br></pre>