<p>NASA's Ultrasonic Crawling Vessel, UCV for short, has arrived to galaxy UDFj - 39546284 in the Fornax constellation and has found a peculiar type of bacteria-like lifeform. As you may imagine a plan to collect samples a bring them back to earth has been set in motion. However, it would be rather unfortunate if they are all dead by the time the UCV gets back, the trip would take approximately 13.42 x 10^9 years travelling at light speed. Therefore, its necessary to pick a number of bacterium so that there are at least some of them alive when the UCV arrives back.</p>
<p><br>The UCV has studied the reproduction cycle of the bacterium inside a cryogenic pod and their behavior when released from the pod, but it lacks the algorithm to compute the final number for such a long period of time. Fortunately, it's been designed with a wormhole plugin installation mechanism that allows to upload algorithms in a matter of only a few years.</p>
<p><br>When the bacterium are inside the cryogenic pod, they follow a very simple reproduction cycle. Every year the following three phases, in order, occur:</p>
<ol>
<li>Aging phase: Each bacteria becomes a year older.</li>
<li>Reproduction phase: Each bacteria gives birth to a new bacteria, this is slightly different to earth bacteria in the sense that the new and old bacterium are no identical. The new bacteria is 0 years old while the old bacteria is at least 1 year old.</li>
<li>Passing phase: Each bacteria that reaches maturity, exactly M years old, dies.</li>
</ol>
<p>Fox example, this one reproduction cycle given a 0 years old bacteria and a 1 years old bacteria if maturity is reached at 2 years old.</p>
<p style="text-align: center;"><img src="../../../content/henu:ucv2013F" alt="Reproduction cicle" width="599" height="172"></p>
<p>As you can see, during cryogenic reproduction, there's no fear of bacterium extintion, the number of births is at least as much as the number of deaths. However, when the pod is opened the bacterium enter into a strange iterative reduction phase, in each step of the reduction the oldest R bacterium die immediately; this process ends when there are fewer than R bacterium left. Note that the biggest problem arises when at some iteration there are exactly R bacterium left because they all die at that moment.</p>
<p>NASA ha asked you to write the algorithm that will be uploaded to the UCV to determine the number of bacterium that will exist after the pod is opened here on earth.</p>
<h3>Input</h3>
<p>The input contains several test cases, each one corresponding to a single simulation. Each test case starts with a line with three integers, the maturity age (1 &lt;=  M &lt;= 50), the number of years for the UCV to come back (0 &lt;= Y &lt;=  10^12) and the reduction size (1 &lt;= R &lt;= 10^9); separated by a single space. The following line contains M integers, they<br>represent the number of 0, 1, ...,M - 1 years old bacterium placed inside the cryogenic pod.</p>
<p><br>The end of input is indicated by a test case with M = Y = R = 0.</p>
<h3>Output</h3>
<p>For each simulation output a single line containing a single integer, the number of bacterium that will be alive after the reduction process has nalized.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 1 4<br>1 1<br>2 1 2<br>1 1<br>2 2 2<br>1 1<br>2 2 5<br>1 1<br>6 0 100000<br>0 1 2 3 4 5<br>6 1000000000000 100000<br>0 1 2 3 4 5<br>0 0 0

<strong>Output:</strong>
3<br>1<br>1<br>0<br>15<br>21809<br>&nbsp;</pre>