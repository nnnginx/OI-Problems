<!-- p { margin-bottom: 0.08in; }h2 { margin-bottom: 0.08in; }pre.cjk { font-family: "DejaVu Sans",monospace; }tt.cjk { font-family: "DejaVu Sans",monospace; } -->
<p style="text-align: center;"><span style="color: #0000a0;"><span style="font-size: large;"><strong>Construction Schedule</strong></span></span></p>
<p>There are many tasks which need to be done in order to construct a building. In order to perform these tasks, there should be a reasonable schedule. There might be relations between tasks. The difficulty we meet in creating a schedule is that the schedule has to satisfy all given relations among the given tasks.</p>
<p>Given a set of tasks and their relations, your task is to write a program to check whether it is possible to create a schedule to perform the tasks.</p>
<h2><a name="SECTION0001001000000000000000"></a><span style="color: #ff0000;"><span style="font-size: medium;">Input&nbsp;</span></span></h2>
<p>The input consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.</p>
<p>For each data set, the first line contains two integer numbers <em>n</em> (1<img src="file://W5aQPf8S.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>n</em><img src="file://ggBovhrS.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">500), and <em>k</em> (0<img src="file://eEA264oU.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>k</em><img src="file://R18BLkMz.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">20000) separated by spaces, where <em>n</em> denotes the total number of tasks, and <em>k</em> denotes the total number of relations. The next <em>k</em> following lines describe <em>k</em> relations among the tasks. Let <em>t</em><sub>j</sub> be a starting time of the task <em>j</em>, <em>j</em> = 1, 2,..., <em>n</em>. Each relation is in one of the two forms:</p>
<ul>
<li>
<p style="margin-bottom: 0in;"><em>x</em>&nbsp;<em>y</em>&nbsp;<em>v</em> means task <em>x</em> must not start after task <em>y</em> starts <em>v</em> days, i.e. <em>t</em><sub>x</sub><img src="file://YomtXVjd.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>t</em><sub>y</sub> + <em>v</em>,</p>
</li>
<li>
<p><em>x</em>&nbsp;<em>y</em>&nbsp; - <em>v</em> means task <em>x</em> must not start before task <em>y</em> starts <em>v</em> days, i.e. <em>t</em><sub>x</sub><img src="file://Rz0dyzZv.png" border="0" alt="$ \ge$" width="18" height="31" align="MIDDLE"><em>t</em><sub>y</sub> + <em>v</em>, where <em>v</em> is a positive integer not greater than 10 	000.</p>
</li>
</ul>
<h2><a name="SECTION0001002000000000000000"></a><span style="color: #ff0000;"><span style="font-size: medium;">Output&nbsp;</span></span></h2>
<p>For each test case, write in one line ``<tt>YES</tt>" if it is possible to construct a schedule to satisfy all the given relations among the given tasks, ``<tt>NO</tt>" otherwise.</p>
<h2><a name="SECTION0001003000000000000000"></a><span style="color: #ff0000;"><span style="font-size: medium;">Sample Input&nbsp;</span></span></h2>
<pre>2 
2 2 
1 2 -2 
1 2 1 
2 1 
1 2 -1</pre>
<h2><a name="SECTION0001004000000000000000"></a><span style="color: #ff0000;"><span style="font-size: medium;">Sample Output&nbsp;</span></span></h2>
<pre>NO 
YES</pre>
<p style="margin-bottom: 0in;">&nbsp;</p>