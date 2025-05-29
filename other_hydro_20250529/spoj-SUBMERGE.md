<p>Vice City is built over a group of islands, with bridges connecting them. As anyone in Vice City knows, the biggest fear of vice-citiers is that some day the islands will submerge. The big problem with this is that once the islands submerge, some of the other islands could get disconnected. You have been hired by the mayor of Vice city to tell him how many islands, when submerged, will disconnect parts of Vice City. You should know that initially all the islands of the city are connected.</p>
<h3>Input</h3>
<p>The input will consist of a series of test cases. Each test case will start with the number N (1 ¡Ü N ¡Ü 10^4) of islands, and the number M of bridges (1 ¡Ü M ¡Ü 10^5). Following there will be M lines each describing a bridge. Each of these M lines will contain two integers Ui, Vi (1 ¡Ü Ui,Vi ¡Ü N), indicating that there is a bridge connecting islands Ui and Vi. The input ends with a case where N = M = 0.</p>
<h3>Output</h3>
<p>For each case on the input you must print a line indicating the number of islands that, when submerged, will disconnect parts of the city.</p>
<h3>Example</h3>
<pre><b><u>Input:</u></b>
3 3
1 2
2 3
1 3
6 8
1 3
6 1
6 3
4 1
6 4
5 2
3 2
3 5
0 0


<b><u>Output:</u></b>
0
1
</pre>