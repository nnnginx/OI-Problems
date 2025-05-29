<p>Mirko and Slavko are training hard for the annual tandem cycling marathon taking place in Croatia. They need to&nbsp;choose a route to train on.&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">There are N cities and M roads in their country. Every road connects two cities and can be traversed in both&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">directions. Exactly N−1 of those roads are paved, while the rest of the roads are unpaved trails. Fortunately, the&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">network of roads was designed so that each pair of cities is connected by a path consisting of paved roads. In&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">other words, the N cities and the N−1 paved roads form a tree structure.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Additionally, each city is an endpoint for at most 10 roads total.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A training route starts in some city, follows some roads and ends in the same city it started in. Mirko and Slavko&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">like to see new places, so they made a rule never to go through the same city nor travel the same road twice.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The training route may start in any city and does not need to visit every city.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Riding in the back seat is easier, since the rider is shielded from the wind by the rider in the front. Because of&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">this, Mirko and Slavko change seats in every city. To ensure that they get the same amount of training, they must&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">choose a route with an even number of roads.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko and Slavko's competitors decided to block some of the unpaved roads, making it impossible for them to&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">find a training route satisfying the above requirements. For each unpaved road there is a cost (a positive integer)&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">associated with blocking the road. It is impossible to block paved roads.&nbsp;Mirko and Slavko are training hard for the annual tandem cycling marathon taking place in Croatia. They need to&nbsp;</div>
<p>There are N cities and M roads in their country. Every road connects two cities and can be traversed in both&nbsp;</p>
<p>directions. Exactly N−1 of those roads are paved, while the rest of the roads are unpaved trails. Fortunately, the&nbsp;network of roads was designed so that each pair of cities is connected by a path consisting of paved roads. In&nbsp;other words, the N cities and the N−1 paved roads form a tree structure.&nbsp;</p>
<p>Additionally, each city is an endpoint for at most 10 roads total.&nbsp;</p>
<p>A training route starts in some city, follows some roads and ends in the same city it started in. Mirko and Slavko&nbsp;like to see new places, so they made a rule never to go through the same city nor travel the same road twice.&nbsp;The training route may start in any city and does not need to visit every city.&nbsp;</p>
<p>Riding in the back seat is easier, since the rider is shielded from the wind by the rider in the front. Because of&nbsp;this, Mirko and Slavko change seats in every city. To ensure that they get the same amount of training, they must&nbsp;choose a route with an even number of roads.&nbsp;</p>
<p>Mirko and Slavko's competitors decided to block some of the unpaved roads, making it impossible for them to&nbsp;find a training route satisfying the above requirements. For each unpaved road there is a cost (a positive integer)&nbsp;associated with blocking the road. It is impossible to block paved roads.</p>
<p>Write a program that, given the description of the network of cities and roads, finds the smallest total cost&nbsp;needed to block the roads so that no training route exists satisfying the above requirements.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input contains two integers N and M (2 ≤ N ≤ 1 000, N−1 ≤ M ≤ 5 000), the number of cities&nbsp;and the total number of roads.&nbsp;</p>
<p>Each of the following M lines contains three integers A, B and C (1 ≤ A ≤ N, 1 ≤ B ≤ N, 0 ≤ C ≤ 10 000),&nbsp;describing one road. The numbers A and B are different and they represent the cities directly connected by the&nbsp;road. If C=0, the road is paved; otherwise, the road is unpaved and C represents the cost of blocking it.&nbsp;</p>
<p>Each city is an endpoint for at most 10 roads. There will never be more than one road directly connecting a&nbsp;single pair of cities.&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output should consist of a single integer, the smallest total cost as described in the problem statement.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 8 
2 1 0 
3 2 0 
4 3 0 
5 4 0 
1 3 2 
3 5 2 
2 4 5 
2 5 1</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5</span></pre>
<pre><span style="font-weight: bold; ">Input:</span></pre>
<pre><span style="font-family: 'courier new', courier;">9 14 
1 2 0 
1 3 0 
2 3 14 
2 6 15 
3 4 0 
3 5 0 
3 6 12 
3 7 13 
4 6 10 
5 6 0 
5 7 0 
5 8 0 
6 9 11 
8 9 0 </span></pre>
<pre><span style="font-weight: bold; ">Output:</span></pre>
<pre><span style="font-family: 'courier new', courier;">48</span></pre>