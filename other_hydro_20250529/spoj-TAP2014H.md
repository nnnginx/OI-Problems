<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2014 in order to have multiple test cases per input file.&nbsp;</strong><span style="font-weight: bold;"><a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a>&nbsp;</span><span style="font-weight: bold;">]</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Nlogonia is a very organized city, where the houses of the inhabitants are all located on the East End of the city and their workplaces are located on the West End.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each working day, people go to their workplaces in the West and at the end of the day they return to their homes in the East. They rely on the urban rail system of Nlogonia for transportation.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The train company offers N different services. Each of them makes a journey that links a station on the West to a station on the East. There are exactly N stations on the West and N stations on the East. At both ends, the stations are numbered from 1 to N following North-South order. The station further north is identified with the number 1 and the station further south with the number N. Each station on both ends belongs to exactly one service.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">[Figura]</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Situation with N = 5 stations corresponding to the first sample input.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">When the workday ends, the Nlogonians leave their workplaces, eager to return home. This results in heavy traffic over the rail system usually known as "rush hour traffic".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">As shown in the figure above, some train services cross over their paths. Two paths cross each other if and only if the relative order of the trains on the North-South direction is different when leaving the West station than when they reach the East station.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">To avoid accidents, Nlogonia's train company decided to schedule the trains departures in shifts so that there are not two trains whose routes intersect leaving on the same shift.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">They want to avoid delays, so their goal is to come up with a schedule such that the number of shifts is minimized.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Luckily, there is exactly one train of each service leaving on rush hour.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Following the example of the previously shown figure, the service departing from station 5 intersects with all the other ones, therefore a shift must be scheduled exclusively for its departure.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The remaining four services cannot be scheduled on a single shift as there are some existing crossings among them. However, it is possible to group them into two shifts, one for trains leaving stations 1 and 2, and another one for trains leaving stations 3 and 4. Thus, a total of 3 shifts will be necessary to avoid any risk of collissions.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You will be responsible for this task: given the descriptions of the N train services in Nlogonia, you must determine the minimum number of turns in which you can plan train departures avoiding any risk of accidents.</div>
<p>Nlogonia is a very organized city, where the houses of the inhabitants are all located on the East End of the city and their workplaces are located on the West End.</p>
<p>Each working day, people go to their workplace in the West and at the end of the day they return to their homes in the East. They rely on the urban rail system of Nlogonia for transportation.</p>
<p>The train company offers <strong>N</strong> different services. Each of them makes a journey that links a station on the West to a station on the East. There are exactly <strong>N</strong> stations on the West and <strong>N</strong> stations on the East. At both ends, the stations are numbered from <strong>1</strong> to <strong>N</strong> following North-South order. The station furthest to the North is identified with the number <strong>1</strong> and the station furthest to the South with the number <strong>N</strong>.&nbsp;On both ends, each station belongs to exactly one service.</p>
<p style="text-align: center;"><img title="Figure 1" src="../../content/fidels:TAP2014H.png" alt="Figure 1"></p>
<p><span style="font-size: xx-small;"><strong>Figure 1: </strong>Situation with <strong>N = 5</strong> stations corresponding to the first sample input.</span></p>
<p>When the workday ends, the Nlogonians leave their workplaces eager to return home. This results in heavy traffic over the rail system usually known as "rush hour traffic".</p>
<p>As shown in Figure 1 above, some train services cross over their paths. Two paths cross each other if and only if the relative order of the trains in the North-South direction is different when leaving the West station than when they reach the East station.</p>
<p>To avoid accidents, Nlogonia's train company decided to schedule the trains' departures in shifts so that there are no two trains whose routes cross leaving on the same shift. They want to avoid delays, so their goal is to come up with a schedule such that the number of shifts is minimized. Luckily, there is exactly one train of each service leaving on rush hour.</p>
<p>Continuing with the example of the previously shown Figure 1, the service departing from station <strong>5</strong> intersects with all the other services, therefore a shift must be scheduled exclusively for its departure. The remaining four services cannot be scheduled on a single shift as there are some crossings among them. However, it is possible to group them into two shifts, one for trains leaving stations <strong>1</strong> and <strong>2</strong>, and another one for trains leaving stations <strong>3</strong> and <strong>4</strong>. Thus, a total of <strong>3</strong> shifts will be necessary to avoid all risk of collissions.</p>
<p>You will be responsible for this task: given the descriptions of the <strong>N</strong> train services in Nlogonia, you must determine the minimum number of turns in which you can plan train departures avoiding all possible risk of accidents.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer number <strong>T</strong>, the number of test cases (<strong>1 �� T �� 200</strong>). <strong>T</strong> test cases follow.</p>
<p>The first line of each test case contains an integer <strong>N</strong> indicating the number of train services in Nlogonia (<strong>1 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong>). The second line contains <strong>N</strong> different integers <strong>E<sub>1</sub>, E<sub>2</sub>, ..., E<sub>N</sub></strong> (<strong>1&nbsp;��&nbsp;E<sub>i</sub>&nbsp;��&nbsp;N</strong>), indicating that the train leaving the <strong>i</strong>-th station on the West should get to station <strong>E<sub>i</sub></strong> on the East, for <strong>i = 1, 2, ..., N</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a line containing a single integer representing the minimum number of turns in which the services can be planned.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3
5
4 5 2 3 1
3
1 2 3
9
9 4 2 7 8 3 5 6 1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
1
4</span></pre>