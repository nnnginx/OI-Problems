<p>In response to a request by the SWERC 2010 problem-setting team, a sensor network has just been installed in the headquarters. The organizing committee has put in the problem-setters the disproportionate fear of suffering a leak of classified information about the problems.</p>
<p>Nevertheless, in the rush they forgot to think about the electricity network needed to make the sensors work. Because of this, the security system is currently not working, but we need to justify the great amount of resources invested in it, so the installation must be ready before the end of the contest. Hence you are now asked to elaborate a program which will help the electrician in his duty.</p>
<p>Since the organizing committee spared no expense, they ordered the sensors from a prestigious company. Every sensor is handcrafted and a number is written on each of them, whose meaning is the recommended voltage that should be applied to it for correct operation. They can be used under higher voltages, with an increasing risk of failure, but never with a voltage below the recommended one. The electrician gazed open-mouthed at the sensors when they were given to him: nearly all of them had different recommended voltages! The sensors were installed in the building in such a way that each of them controls exactly two doors and every door is controlled by at least one sensor. Now is the time for the electrician to supply power to the sensors. He faces the following constraints:</p>
<ul class="itemize">
<li class="li-itemize">Fortunately, there is no need to activate all sensors. However, we will require that the subset of sensors chosen to be on satisfy that every door is controlled by, at least, one sensor in the subset.</li>
<li class="li-itemize">Electricity is to be supplied to one of the active sensors, and then distributed to the others with wires. In order not to waste wires, they can only be installed by connecting a pair of neighboring active sensors (by “neighbouring” we mean that some door is controlled by both of them). Since we must supply energy to every active sensor, not every subset of sensors is suitable as the chosen subset of working sensors.</li>
<li class="li-itemize">Because of the above, all of the sensors will be supplied the same voltage, which cannot be below the corresponding recommended voltages.</li>
</ul>
<p>For simplicity, we will refer to a subset of sensors satisfying the first two constraints above as an admissible subset. The network is designed so that the set of all sensors is always admissible, but we would like to take a possibly smaller subset so as to minimize the <em>margin</em>, defined as the maximum of the differences, in absolute value, between the numbers written on each pair of sensors in the subset. (This is to keep the chances of failure to a minimum).</p>
<p>The electrician could not solve the task of finding the admissible subset of the set of sensors for which the margin is minimum. Therefore, the electrical installation is still missing. Today, we ask you to write a program to find out the answer, given a sensor network and the recommended voltage for each of the sensors.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of several test cases, separated by single blank lines. Each test case begins with a line containing the integer <em>n</em> (2 ≤ <em>n</em> ≤ 350), the number of doors in the building. The following line contains another integer, <em>m</em> (<em>n</em> − 1 ≤ <em>m</em> ≤ <em>n</em> (<em>n</em> − 1) / 2), the number of sensors in the network. The test case finishes with <em>m</em> lines containing a description of each of the <em>m</em> sensors. The <em>i</em>-th of those lines contains three integers, <em>a</em> (0 ≤ <em>a</em> ≤ <em>n</em> − 1), <em>b</em> (0 ≤ <em>b</em> ≤ <em>n</em> − 1) and <em>w</em> (1 ≤ <em>w</em> ≤ 2<sup>15</sup>), in that order. Integers <em>a</em> and <em>b</em> represent the pair of doors controlled by the <em>i</em>-th sensor, and <em>w</em> its recommended voltage. You can safely assume that there are no two sensors controlling the same two doors.</p>
<p>The input will finish with a line containing <tt>0</tt>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each case, your program should output a line containing the minimum margin of an admissible subset of the sensors.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3
3
0 1 220
1 2 120
2 0 160

4
5
2 3 80
1 3 80
0 1 180
2 1 200
3 0 140

0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">40
60
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Luis Hernández Corbato</em></blockquote>
</div>