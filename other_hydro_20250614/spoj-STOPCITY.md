<p>You work for a tour operator which plans to commercialize different visiting tours in a country. A tour is a sequence of cities that are visited during the trip. A city cannot be visited more than once in one tour. Each city is represented as a node in a non-oriented graph where edges are possible connections. Given a departure city A and a destination city B, we call stopping-off-city a city that is part of at least one possible tour between A and B. Your mission is to select all possible stopping-off-cities between A and B. In the example of the figure bellow, we have a graph of 20 cities. If we consider the departure as node 10 and the arrival as node 16 the stopping-off-cities are {8, 9, 10, 11, 12, 13, 15, 16}.</p>
<p><img src="../../../content/nils75:stopcity" alt=""></p>
<h3>Input</h3>
<p>First line of input consists of an integer V denoting the number of nodes or cities (V&lt;=10000). Then, each line contains an edge definition as two space separated integers (link between two cities).  Edges description ends with the line "-1 -1" (without cotes). The last line contains two space separetad integers "<em><strong>s d</strong></em>" where <em><strong>s</strong></em> is the departure city and <em><strong>d</strong></em> the destination city.</p>
<h3>Output</h3>
<p>A space separated sorted list of stopping-off-cities including <em><strong>s</strong></em> and <em><strong>d</strong></em>.&nbsp; It is guaranteed that atleast one path exists between <strong style="font-weight: bold;"><em>s</em></strong><span style="font-weight: bold;"> and&nbsp;<strong style="font-weight: bold;"><em>d</em></strong></span>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
20
0 1
1 2
2 3
3 4
4 5
5 6
6 7
1 8
8 11
8 9
9 10
11 12
9 12
12 13
12 15
12 14
14 19
14 18
14 17
17 18
18 19
13 15
15 16
-1 -1
10 16

<strong>Output:</strong>
8 9 10 11 12 13 15 16
</pre>