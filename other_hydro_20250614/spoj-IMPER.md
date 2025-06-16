<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>The ambition of conquest and expansion is a very well known  disease in planet Earth... and also in the entire universe.</p>
<p>In planet ��Imperius�� several fortresses have been  built one at a time and each one of them but the first was connected  at the moment of its construction to a previously built fortress by a  direct path, for commercial purposes.</p>
<p>Imperius was becoming one of the most peaceful and prosperous  planet in the universe, until they built no more fortresses. At that  moment, <strong>N</strong> different empires emerged (numbered from 1 to <strong>N</strong>), each one  of them dominating a different fortress. And the thirst of conquest  took Imperius. Thus, every year, exactly one of the living empires  conquers every neighbor empire, and dominates every fortress  belonging to them. Two empires are considered neighbors if there  exist two fortresses joined by a path, each one dominated by one  different empire of these two.</p>
<p>Eventually a single empire will dominate every fortress. Your task is  to find the minimum number of years such that this can happen.</p>
<p>As an example, on the left side of the figure below a possible  scenario in which six fortresses are initially dominated by six  different empires is shown. Each fortress is tagged with the  identification number of the empire dominating it. If empire 2  conquered every neighbor on the first year, the the situation would  be as in the central figure. Finally, if empire 5 conquered his  neighbor empires, it would end up dominating every fortress, as seen  on the right side of the figure.</p>
<p><img src="../../../content/pabloh:taip2011I1.png" alt="" width="25%"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="../../../content/pabloh:taip2011I2.png" alt="" width="25%"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="../../../content/pabloh:taip2011I3.png" alt="" width="25%"></p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described  in two lines. The first line contains an integer <strong>N</strong> (2 &lt;= <strong>N</strong> &lt;=  10<sup>4</sup>) representing the number of fortresses in planet Imperius. The  next line contains <strong>N</strong>-1 integers <strong>P_i</strong> indicating that the fortress <strong>i</strong>+1 was connected to fortress <strong>P_i</strong> (1 &lt;= <strong>P_i</strong> &lt;= <strong>i</strong> for 1 &lt;= <strong>i</strong> &lt;= <strong>N</strong>-1).  The last line of the input contains a single -1 and  should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case output a single line with an integer  representing the minimum number of years such that a single empire may dominate every fortress.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>6
1 2 2 4 5
7
1 1 3 3 4 4
6
1 2 2 2 2
-1</pre>
<p><strong>Output:</strong></p>
<pre>2
2
1</pre>