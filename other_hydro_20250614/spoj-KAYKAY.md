<p><span style="font-family: 'courier new', courier;"><br></span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Given a tree - &nbsp;A connected and acyclic graph with n vertices.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Each node in the tree has a value associated with it.&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Given a set of vertices S, value(S) = sum of values of all vertices in set S.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Your task is to select two components A and B such that:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">1. A and B are disjoint (they have no vertex in common)</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">2. A has k1 vertices; i.e, | A | = k1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">3. B has k2 vertices; i.e, | B | = k2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">4. value(A) - value(B) is maximized.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">If it is not possible to select two such components, print -1.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Constraints:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">n &lt;= 500</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">k1, k2 &lt;= n</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Input:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">First line contains t, total test cases.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Each test case is as follows:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">First line contains three integers: n, k1 and k2.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Next line contains n integers, the values of the n nodes; -100000 &lt;= value &lt;= 100000</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Next n - 1 lines contain 2 integers a and b, indicating that there is an edge between a and b. 0 &lt;= a &lt; b &lt; n</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Output:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">For each test case, print one line containing an integer = | value(A) - value(B) |.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Sample Input:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">7 3 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">0 1 -1 2 3 -2 -3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">1 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">1 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">2 4</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">2 5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">3 6</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">3 7</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">3 2 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">1 2 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">0 1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">0 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">Sample Output:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">12</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-family: 'courier new', courier;">-</span></div>
<p><span style="font-family: 'courier new', courier;">The CSE Department of NIT Trichy is not particularly reknowned for its eye-candy. Noticing this, Paarth decides to distribute some candies throughout the department. The department consists of n rooms. There are corridors connecting certain pairs of rooms. Being very frugal, the corridors are designed in such a way that every pair of rooms are connected by exactly one path. Now Alpa and Syed are let loose in the department and they want to collect as many candies as possible. Alpa has hired you to help him maximize the difference between the number of candies obtained by him and Syed based on the constraint that he shall never enter any room that is visited by Syed. </span></p>
<p>&nbsp;</p>
<p><span style="font-family: 'courier new', courier;">More formally, you are given a tree - &nbsp;A connected and acyclic graph with n vertices.</span></p>
<p><span style="font-family: 'courier new', courier;">Each vertex in the tree has a value associated with it (the number of candies). Note that the number of candies may be negative as well (bullies waiting to snatch your candies away)&nbsp;</span></p>
<p><span style="font-family: 'courier new', courier;">Given a set of vertices S, value(S) = sum of values of all vertices in set S.</span></p>
<p><span style="font-family: 'courier new', courier;">Your task is to select two sets of vertices A and B such that:</span></p>
<p><span style="font-family: 'courier new', courier;">1. A and B are disjoint (they have no vertex in common)</span></p>
<p><span style="font-family: 'courier new', courier;">2. Every vertex in A is connected to every other vertex in A through some path;&nbsp;</span></p>
<p><span style="font-family: 'courier new', courier;">3. Every vertex in B is connected to every other vertex in B through some path;&nbsp;</span></p>
<p><span style="font-family: 'courier new', courier;">4. A has k1 vertices; i.e, | A | = k1</span></p>
<p><span style="font-family: 'courier new', courier;">5. B has k2 vertices; i.e, | B | = k2</span></p>
<p><span style="font-family: 'courier new', courier;">6. value(A) - value(B) is maximized.</span></p>
<p>&nbsp;</p>
<p><span style="font-family: 'courier new', courier;">If it is not possible to select two such components, print -1.</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong><span style="font-family: 'courier new', courier;">Constraints:</span></strong></p>
<p><span style="font-family: 'courier new', courier;">2 &lt;= n &lt;= 200</span></p>
<p><span style="font-family: 'courier new', courier;">0 &lt; k1, k2 &lt;= n</span></p>
<p><span style="font-family: 'courier new', courier;">Values of all vertices are between -10 ^ 5 and 10 ^ 5</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong><span style="font-family: 'courier new', courier;">Input:</span></strong></p>
<p><span style="font-family: 'courier new', courier;">First line contains t, total test cases.</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;</span><span style="font-family: 'courier new', courier;">Each test case is as follows:</span></p>
<p><span style="font-family: 'courier new', courier;">First line contains three integers: n, k1 and k2.</span></p>
<p><span style="font-family: 'courier new', courier;">Next line contains n integers, the values of the n vertices.</span></p>
<p><span style="font-family: 'courier new', courier;">Next n - 1 lines contain 2 integers a and b, </span></p>
<p><span style="font-family: 'courier new', courier;">indicating that there is an edge between vertices a and b; 0 &lt;= a &lt; b &lt; n</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong><span style="font-family: 'courier new', courier;">Output:</span></strong></p>
<p><span style="font-family: 'courier new', courier;">For each test case, print one line containing an integer = value(A) - value(B) .</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong><span style="font-family: 'courier new', courier;">Sample Input:</span></strong></p>
<p><span style="font-family: 'courier new', courier;">2</span></p>
<p><span style="font-family: 'courier new', courier;">7 3 3</span></p>
<p><span style="font-family: 'courier new', courier;">0 1 -1 2 3 -2 -3</span></p>
<p><span style="font-family: 'courier new', courier;">0 1</span></p>
<p><span style="font-family: 'courier new', courier;">0 2</span></p>
<p><span style="font-family: 'courier new', courier;">1 3</span></p>
<p><span style="font-family: 'courier new', courier;">1 4</span></p>
<p><span style="font-family: 'courier new', courier;">2 5</span></p>
<p><span style="font-family: 'courier new', courier;">2 6</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><span style="font-family: 'courier new', courier;">3 2 2</span></p>
<p><span style="font-family: 'courier new', courier;">1 2 3</span></p>
<p><span style="font-family: 'courier new', courier;">0 1</span></p>
<p><span style="font-family: 'courier new', courier;">0 2</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong><span style="font-family: 'courier new', courier;">Sample Output:</span></strong></p>
<p><span style="font-family: 'courier new', courier;">12</span></p>
<p><span style="font-family: 'courier new', courier;">-1</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><strong>Explanation:</strong></p>
<p><span style="font-family: 'courier new', courier;">In the first case, A = { 1, 3, 4}; B = {2, 5, 6}.</span></p>