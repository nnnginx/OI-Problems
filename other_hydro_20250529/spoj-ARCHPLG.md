Byteland is a country located in the Archipelago of Rectangular Islands. The archipelago consists of <tt>1&lt;=n&lt;=1000</tt> islands. A fact that each island has a rectangular shape is very nice for Bytelandian cartographers. 
<p>

</p><p>
Bytelandian islands are rather small and none are very fertile, so each of (rectangular of course) pieces of cultivated land is under special control, simply speaking: ��never enter there to save your life��. Other areas are guaranteed to be free accessible for the people.

</p><p>
The communication between islands is possible by ferries. On each island there is <tt>0&lt;=b&lt;=10</tt> terminals, from where crossings to another terminals on other islands are possible. 
It is known that total number of crossing connections is <tt>0&lt;=m&lt;=100000</tt>. Other infrastructure is practically unknown. Specifically the only possible 
way of traveling through  the island is to do it on foot. 

</p><p>
Well, now we are close to a task you are requested to solve. John �C one of the Bytelandian citizens is working as a sales manager. Simply speaking he is often requested to travel from one place to another, what he rather dislike and preferably (like other Bytelandian people use to do) he would like to spent more time in one of the
beach clubs playing Puto (a kind of strategic game, very popular in Byteland). Please help him to find a way to spare his time.

</p><h3>Task</h3>
<p> Find one of the fastest ways for John using ferries and foot paths on islands. Assume that while walking John is always moving one BM (Bytelandian unit of length) per BH  (Bytelandian unit of time). 
You can also assume that the ferry departures nearly immediately after John arrives the terminal, it will be enough to round up the walking time to the nearest integer.

</p><h3>Input</h3>
<p>In the first  line <tt>t</tt> - the number of tests, then for each test:
in next line <tt>n</tt> - the number of islands. Description of each island is as follows:
</p><pre>name
w h [island dimensions]
b - [number of terminals]
[description of each terminal in a form:]
name x y [name of a terminal and its coordinates]
F [number of restricted areas F&lt;20]
xl, yd, xr, yu [coordinates of each restricted area,
0 &lt;=xl &lt; xr&lt;=250 0&lt;=yd &lt; yu&lt;=250.]
</pre>
<p>
All coordinates are nonnegative integers measured in BM according to upper left corner of an island.

</p><p>
You can assume that any two restricted areas are disjoint. After the description of all islands all ferry connections are given (each connection is bi-directional). 
</p><pre>m  [number of connections]
[description of each connection]
NB1 NW1 NB2 NW2 time [name of a first terminal, its island, the second respectively
and communiaction time]
...
[description follows]
...
NBS NWS NBC NWC [start and goal terminal for John]
</pre>

<h3>Output</h3>
<p>
For each test describe the shortest route for John from terminal NBS on NWS island to terminal  NBC on NWC island in the following format:
</p><pre>case nr Y [nr - test number]
T [travel time in BH]
NBS  NWS
...
[consecutive terminals]
...
NBC NWC
[empty line]
[consecutive tests]
</pre>
<p>
If two consecutive terminals are located on the same island and John must take some walk you must give all middle point like in an example.

</p><p>
<img src="/content/kuszi:trectarch_example.png" width="100%">


</p><h3>Example</h3>

<pre><b>Input:</b>
1
3
W1
8 7
2
Lindos 4 0
Kamejros 4 7
3
2 1 6 2
2 3 6 4 
2 5 6 6 
W2
14 12
2
Malia 14 1
Knossos 1 12
5
2 6 10 10
11 1 12 6
8 1 10 5
11 7 12 9
3 2 5 4
W3 
1 1
1
Korkyra 0 0
0
2
Kamejros W1 Knossos W2 100
Malia W2 Korkyra W3 100
Korkyra W3 Lindos W1
</pre>
<p>
An example of a correct answer:
</p><pre><b>Output:</b>
case 1 Y
230
Korkyra W3
Malia W2
12 6
11 7
10 10
Knossos W2
Kamejros W1
2 6
2 1
Lindos W1
</pre>