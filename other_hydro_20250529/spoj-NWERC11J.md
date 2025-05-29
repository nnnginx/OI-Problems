<h3>  Train delays</h3>
<!--l. 3-->
<p>Last year, some of the judges tried to travel to NWERC¡¯10 by train. This turned into a big disaster: on the way there, a fire in a control room caused huge delays, while on the return trip, trains in Bremen were delayed due to a terrorist threat in Hamburg. Of course, these huge delays caused other delays in the train schedule, so the big question was which trains to take: would it be better to take this slow regional train now, or wait for that intercity train, which has a big chance of being delayed? <!--l. 12--></p>
<p>This year, the judges have planned ahead and carefully analyzed the train schedule. They even kept track of how often trains were delayed and by how much. Now that they have all this information, they want to travel as quickly possible, minimizing the expected duration of the journey. Can you help them? <!--l. 18--></p>
<p>For each train connection, the judges know exactly what its scheduled departure time and duration are, as well as the probability that its arrival at the destination will be delayed. You may assume that the probabilities of delays are independent and that the judges can adapt their itinerary as they go, depending on any delays which they might already have incurred. Trains always depart on time, but may arrive late and the judges do not know whether a train¡¯s arrival will be delayed until they have boarded it. It takes judges no time to switch trains, so they can take a connecting train that departs at the same time as they arrive at a place. <!--l. 31--></p>
<p>The judges can choose the time of their initial departure as they wish and they want to minimize the expected duration<a id="fn1x0-bk" href="#fn1x0"><sup>1</sup></a> of their total trip. <!--l. 40--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 41-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with the judges¡¯ place of origin and destination, these are different. </li>
<li>one line with an integer <em>n </em>(1 ¡Ü <em>n </em>¡Ü 1<span style="margin-left:0.3em">&nbsp;000): the number of train connections. </span></li>
<li><em>n </em>lines, each describing a train connection:             
<ul>
<li>the origin and destination of this connection, these are different. </li>
<li>an integer <em>m </em>(0 ¡Ü <em>m </em>¡Ü 59), the departure time in minutes after each full hour. </li>
<li>an integer <em>t </em>(1 ¡Ü <em>t </em>¡Ü 300), the standard journey time (assuming no delays). </li>
<li>an integer <em>p </em>(0 ¡Ü <em>p </em>¡Ü 100), the probability of delays as a percentage. </li>
<li>an integer <em>d </em>(1 ¡Ü <em>d </em>¡Ü 120), the maximum delay in minutes.</li>
</ul>
</li>
</ul>
<!--l. 63-->
<p>All place names are given as strings of upper and lower case alphabetical characters, of length at most 20. If a train is delayed, then the length of the delay will be a whole number of minutes, and will be uniformly distributed in the range [1<em>,d</em>]. <!--l. 68--></p>
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 69-->
<p>Per test case:</p>
<ul>
<li>one line with a floating point number: the minimum expected duration of the total       trip in minutes.</li>
</ul>
<!--l. 74-->
<p>This number should be accurate up to 10<sup>-6</sup> relative or absolute precision. Output <tt>IMPOSSIBLE</tt> instead if the destination is not reachable. <!--l. 78--></p>
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>3
Hamburg Bremen
3
Hamburg Bremen 15 68 10 5
Hamburg Bremen 46 55 50 60
Bremen Frankfurt 14 226 10 120
Amsterdam Rotterdam
1
Amsterdam Utrecht 10 22 5 10
BremenVegesack Utrecht
9
BremenVegesack BremenHbf 15 10 0 1
BremenVegesack BremenHbf 45 10 0 1
BremenVegesack Leer 23 140 10 15
BremenHbf Osnabruck 44 51 60 70
Osnabruck Amersfoort 55 147 38 40
Amersfoort Utrecht 24 15 30 15
Amersfoort Utrecht 54 15 10 35
Leer Groningen 45 140 5 10
Groningen Amersfoort 46 96 10 20</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>68.3
IMPOSSIBLE
305.0532857 </pre>
</td>
</tr>
</tbody>
</table>
<p>Note in the first example that it is better to take the slower train from Hamburg to Bremen, since the fast train would give an expected travel time of 70<em>.</em>25 minutes.</p>
<hr>
<p><a id="fn1x0" href="#fn1x0-bk"><sup>1</sup></a>Given a travel plan of which trains to take (depending on previous connections and delays), the expected trip duration E is defined to be the sum of the trip duration T<sub>i</sub> for each itinerary i possibly taken multiplied by the chance p<sub>i</sub> of that itinerary occurring: E = ¡Æ <sub>i</sub>p<sub>i</sub><span style="margin-left:0.3em">&nbsp;T<sub>i</sub>.</span></p>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>