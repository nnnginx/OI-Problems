<p>Believe it or not, the devices measuring time in alpine ski racing are not perfect. Instead of measuring the exact time, they measure an interval in which the ski racer finished the race (for example 53.42 sec - 53.45 sec).</p>
<p>The probability is distributed evenly on this interval. <span style="font-size: xx-small;">(More precisely, if we choose any two sub-intervals of equal length, the probability that the ski racer finished the race in each of these sub-intervals is equal. One can also say that each moment in the given interval has equal probability assigned to it, but this in fact says nothing since the probability for each moment is equal to zero (since there are infinitely many moments in the interval) no matter how we distribute the probability.)</span></p>
<p>And what if there are N ski racers? Then we have N intervals. Find the probability that the first ski racer on the list won the race (that is, finished the race with the minimal time).</p>
<h3>Input</h3>
<p>In the first line, there is an integer N (1 ��&nbsp;N �� 300).</p>
<p>In the next N lines, read the intervals assigned to the ski racers: two real numbers A<sub>i</sub>&nbsp;and B<sub>i</sub>&nbsp;in each line, representing the interval [Ai, Bi] of the i-th ski racer. (0 &lt; A<sub>i&nbsp;</sub>&lt; B<sub>i&nbsp;</sub>&lt; 1000)</p>
<h3>Output</h3>
<p>Print the required probability. The absolute difference between yours and official solution may be&nbsp;at most 10<sup>-6</sup>.</p>
<h3>Example</h3>
<p><span style="font-weight: bold;"><span style="font-size: x-small;">input</span></span></p>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">2
1.000 5.000
2.500 3.000
</pre>
<p><span style="font-weight: bold;"><span style="font-size: x-small;">output</span></span></p>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">0.437500</pre>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;"><strong><br></strong></pre>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;"><span style="font-size: small;"><strong>input</strong></span></pre>
<pre><pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">4
3.500 17.300
12.700 21.200
2.900 15.000
1.000 20.000
</pre>
<span style="font-weight: bold;"><span style="font-size: medium;">output</span></span>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">0.263541</pre>
</pre>