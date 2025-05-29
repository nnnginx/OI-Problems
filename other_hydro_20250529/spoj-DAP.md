<h3>Description</h3>
<p>You¡®ve been given a N¡ÁN matrix {W_ij} containing the cost of a weighted bipartite graph, on this graph, you need to implement the following operations:</p>
<ul>
<li>C i j w : Change Wij to w.</li>
<li>X i x0 x1 ... xn-1 : Change all Wij to xj.</li>
<li>Y i y0 y1 ... yn-1 : Change all Wji to yj.</li>
<li>A : Add a new pair of node to the current bipartite graph, then increase N by 1. The weight of those 2n+1 new edges will be set to 0 by default.</li>
<li>Q : Query the current maximum weighted matching.</li>
</ul>
<h3>Input</h3>
<p>N <br>(.. . following the N¡ÁN matrix .. .) <br>M<br>(.. . following the M operation .. . .. . )</p>
<h3>Output</h3>
<pre>... <br>(for each query, simply print the result. )</pre>
<h3>Example</h3>
<pre><pre style="text-align: left;"><strong>Input 1:</strong><br>2<br>1 0<br>0 1<br>3<br>Q<br>C 0 1 9<br>Q<br><br><strong>Output 1:</strong><br>2<br>9<br><strong><br>Input 2:<br></strong>10<br>76 98 80 30 87 84 78 75 53 26 <br>85 7 83 15 21 91 47 84 82 78 <br>36 39 49 64 71 14 53 2 82 21 <br>83 31 32 30 78 19 46 95 50 55 <br>50 76 63 54 99 55 50 16 29 26 <br>58 74 77 32 3 91 90 18 34 3 <br>56 23 2 78 84 83 71 41 32 54 <br>53 75 39 29 61 25 42 79 58 2 <br>19 13 65 94 9 33 61 5 1 70 <br>34 56 45 37 72 98 47 40 80 79 <br>20<br>Q<br>Y 3 62 90 89 41 58 56 34 55 53 53<br>X 0 7 30 30 76 2 48 8 18 89 88<br>Q<br>C 2 0 3<br>C 3 0 0<br>C 8 0 2<br>C 1 0 3<br>C 1 0 6<br>C 5 0 9<br>Q<br>A<br>X 10 93 8 56 40 4 56 30 32 59 11 52<br>Y 10 84 62 26 13 66 21 53 23 54 81 52<br>Q<br>Y 9 13 38 99 50 20 25 59 7 6 77 82<br>C 4 0 8<br>C 6 0 6<br>C 10 0 8<br>Q<br><strong><br>Output 2:</strong><br>870<br>849<br>844<br>844<br>839</pre>
</pre>
<h3>Restriction</h3>
<p>We guarantee the N will never be more than 100 even during the running time .. . <br>The total operation M will less than 10000, and among them the Query Operation will less than 1000 .. .</p>