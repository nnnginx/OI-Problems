<p>Townsville has a well developed bus system. Since most of the important buildings in town are located along the Main Street, almost all the buses pass through the street. All the stops along the Main Street, and there are very many of them, are numbered with numbers: 0, 1, 2 and so on. All the buses enter the Main Street at the stop numbered 0 and continue towards the higher numbered stops. For each bus line (which is also identified by a number), there is a schedule posted at stop 0 giving the minutes within an hour when a bus of this line leaves the stop.</p>
<p>Rahul arrives at stop 0 at m minutes (0 &lt;= m &lt; 60) after the hour and takes the first bus that leaves stop 0 along the Main Street. If Rahul arrives at stop 0 the same minute when a bus leaves, Rahul manages to board the bus. He leaves the bus at the next stop and takes the next bus that arrives and continues to the next stop where he leaves. Rahul continues in this fashion until he reaches stop n, 0 &lt; n &lt; 10^9. Your task is to find by which bus will Rahul arrive at stop n?</p>
<h3>Input</h3>
<p>Input contains multiple cases. The first line of a case gives t, the number of bus lines, 0 &lt; t &lt; 30. The next t lines each contain a number of a bus line followed by a colon and then a list (separated by spaces) of minutes after a full hour when the bus of this line leaves stop 0. Each list of departure times is terminated by -1. No bus leaves stop 0 more than 20 times in an hour, no two buses leave station 0 at the same time, all the buses have the same speed and they never meet at a stop. A line with m and n then follows. The input ends with a line where t = 0. This line should not be processed.&nbsp;</p>
<h3>Output</h3>
<p>For each case of input, output in a format shown below the number of the bus line by which Rahul arrives at stop n.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1
11: 10 20 30 -1
3 2
2
11: 10 20 30 -1
134: 16 25 35 45 58 -1
48 783
0</p>
<strong>Output:</strong>
<p>Case 1: Rahul arrives at stop 2 by bus 11.
Case 2: Rahul arrives at stop 783 by bus 134.</p></pre>