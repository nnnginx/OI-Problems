<p style="text-align: justify;">Last week¡¯s campaign on healthy and environmentally friendly mobility was a big success. Hundreds of commuters to the EPFL campus traded their car for a ride by bus or metro and gave a very positive feedback. They merely complained about earlier wake-up times necessary to reach the campus on time.</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/imuteb:ontime.jpg" alt="" width="405" height="202"></p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">This is where you enter the story. Try to improve the mood of the people by indicating them the latest time they can leave their house such that they can reach the campus no later than 8h15. Any means are ok to maximize their sleeping time, and all would accept to change bus or metro lines several times during their journey if this helps your planning.</p>
<p style="text-align: justify;">The public transport network is made up of <em>S (0&lt;=S&lt;=100)&nbsp; </em>stations (numbered from 1 to <em>S</em>) and counts <em>C (0&lt;=C&lt;=1'000)</em>&nbsp; unidirectional connections that link two stations in regular time intervals, starting from a certain time in the morning and up to 8h15. Note that for any two stations, there might exist several direct shuttle services with different starting time and frequency. You are to answer some students¡¯ request on the latest possible time they can leave from home in order not to be late.</p>
<p style="text-align: justify;">&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases separated by an empty line. Each test-case starts with the number of stations <em>S</em>, the number of connections <em>C</em> and the number of requests <em>R</em> on a line. Then come <em>C </em>lines, each describing one shuttle service in the format ¡®from¡¯ ¡®to¡¯ ¡®firstRide¡¯ ¡®travelTime¡¯ ¡®frequency¡¯ (in minutes). The next <em>R</em> lines each hold two integers, the first being the closest station to the student¡¯s home (come what may, but so early no student would like to walk more than necessary) and the second the time (in minutes) it takes the student to reach that station. The campus is located at station <em>S</em>. Input terminates on a test-case <em>with S=C=R=0</em>, which must not be evaluated.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>Answer the requests in the same order as they appeare in the input. For each request, print a line in the form ¡°Leave no later than ¡®time¡¯¡±, where ¡®time¡¯ is in the format <em>hh:mm</em>. Add an empty line after each test-case. If there is no way the students can make it on time, output ¡°Doomed to be late¡±. You can safely assume that the commuters are so experienced in hopping on and off busses that they can change busses in no time at all.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p><span style="font-family: courier new,courier;">3 2 2</span></p>
<p><span style="font-family: courier new,courier;">1 3 07:10 50 15</span></p>
<p><span style="font-family: courier new,courier;">2 3 08:20 5 5</span></p>
<p><span style="font-family: courier new,courier;">1 3</span></p>
<p><span style="font-family: courier new,courier;">2 0</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><span style="font-family: courier new,courier;">3 4 3</span></p>
<p><span style="font-family: courier new,courier;">2 3 05:30 6 5</span></p>
<p><span style="font-family: courier new,courier;">1 3 06:11 5 15</span></p>
<p><span style="font-family: courier new,courier;">1 2 07:01 2 5</span></p>
<p><span style="font-family: courier new,courier;">3 2 08:00 1 8</span></p>
<p><span style="font-family: courier new,courier;">1 2</span></p>
<p><span style="font-family: courier new,courier;">2 1</span></p>
<p><span style="font-family: courier new,courier;">3 10</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><span style="font-family: courier new,courier;">0 0 0&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p><span style="font-family: courier new,courier;">Leave no later than 07:22</span></p>
<p><span style="font-family: courier new,courier;">Doomed to be late</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><span style="font-family: courier new,courier;">Leave no later than 07:59</span></p>
<p><span style="font-family: courier new,courier;">Leave no later than 08:04</span></p>
<p><span style="font-family: courier new,courier;">Leave no later than 08:05</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>