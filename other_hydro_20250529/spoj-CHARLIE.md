<p>Charlie works in a magical chocolate factory.&nbsp;Packets of its marzipan are made on conveyor belts.&nbsp;To make marzipan perfect, M conveyor belts are used, and the process is as follows.</p>
<p>Each of the M belts has N cells.&nbsp;Charlie first makes a few initial packets and puts them on the cells of the first belt (there may be zero or more packets in a particular cell).</p>
<p>Then the first belt generates a second belt such that each cell of the second belt, at the same time, counts the packets in some five cells of the first belt and creates that number of packets in itself.</p>
<p>Fox example, the first cell of the second belt sums the packets in the cells 1, 2, 3, 5, 9 of the first belt, the second cell of the second belt sums the packets in the cells 2, 3, 4, 5, 6 of the first belt and so on.</p>
<p>Then, from the second belt, a third belt is generated in the same manner, then the fourth from the third and so on until the M<sup>th</sup>.&nbsp;Since the number of packets on the belts usually increases, the number of packets in each cell is observed only modulo 10007.</p>
<p>You, as the winner of the golden ticket to the factory, are able to see how the M<sup>th</sup>&nbsp;belt looks like - that is, how many packets of marzipan there is in each cell. Charlie has also explained to you the production process and now you are wondering how first belt looked like.</p>
<h3>Input</h3>
<p><span title="Kliknite za alternativne prijevode">The first</span>&nbsp;<span title="Kliknite za alternativne prijevode">line</span>&nbsp;<span title="Kliknite za alternativne prijevode">of input contains</span>&nbsp;positive&nbsp;<span title="Kliknite za alternativne prijevode">integers</span>&nbsp;<span title="Kliknite za alternativne prijevode">N</span>&nbsp;<span title="Kliknite za alternativne prijevode">(</span><span title="Kliknite za alternativne prijevode">N</span>&nbsp;<span title="Kliknite za alternativne prijevode">��</span>&nbsp;<span title="Kliknite za alternativne prijevode">100)</span>&nbsp;<span title="Kliknite za alternativne prijevode">and</span>&nbsp;<span title="Kliknite za alternativne prijevode">M</span>&nbsp;<span title="Kliknite za alternativne prijevode">(</span><span title="Kliknite za alternativne prijevode">M</span>&nbsp;<span title="Kliknite za alternativne prijevode">&lt;&nbsp;</span><span title="Kliknite za alternativne prijevode">2<sup>31</sup>)</span><span title="Kliknite za alternativne prijevode">.</span></p>
<p>The next N lines describe the process of generating each new belt. In the A<sup>th</sup> of these lines there are five distinct integers from the interval [1, N], denoting the cells of a previous belt from which the packets are added to the A<sup>th</sup> cell of a new belt.</p>
<p><span title="Kliknite za alternativne prijevode">The next</span>&nbsp;<span title="Kliknite za alternativne prijevode">line</span>&nbsp;<span title="Kliknite za alternativne prijevode">contains N</span>&nbsp;<span title="Kliknite za alternativne prijevode">integers</span>&nbsp;<span title="Kliknite za alternativne prijevode">describing the</span>&nbsp;<span title="Kliknite za alternativne prijevode">state of</span>&nbsp;<span title="Kliknite za alternativne prijevode">the</span>&nbsp;<span title="Kliknite za alternativne prijevode">M<sup>th</sup> belt</span>&nbsp;<span title="Kliknite za alternativne prijevode">(</span><span title="Kliknite za alternativne prijevode">modulo</span>&nbsp;<span title="Kliknite za alternativne prijevode">10007</span><span title="Kliknite za alternativne prijevode">)</span><span title="Kliknite za alternativne prijevode">.</span></p>
<h3>Output</h3>
<p><span title="Kliknite za alternativne prijevode">Print</span>&nbsp;<span title="Kliknite za alternativne prijevode">N</span>&nbsp;integers&nbsp;<span title="Kliknite za alternativne prijevode">describing the</span>&nbsp;<span title="Kliknite za alternativne prijevode">state of</span>&nbsp;<span title="Kliknite za alternativne prijevode">the first belt&nbsp;</span><span title="Kliknite za alternativne prijevode">(</span><span title="Kliknite za alternativne prijevode">modulo</span>&nbsp;<span title="Kliknite za alternativne prijevode">10007</span><span title="Kliknite za alternativne prijevode">)</span><span title="Kliknite za alternativne prijevode">.</span>&nbsp;A&nbsp;<strong>unique</strong>&nbsp;solution will exist in all of the test data.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="font-size: 12px; text-align: left; color: #000000; font-family: 'Courier New', Courier, monospace; margin: 8px;">6 3
1 2 3 4 5
1 2 3 4 6
1 2 3 5 6
1 2 4 5 6
1 3 4 5 6
2 3 4 5 6
13 12 12 12 14 12</pre>
<strong>Output:</strong>
<pre style="font-size: 12px; text-align: left; color: #000000; font-family: 'Courier New', Courier, monospace; margin: 8px;"><pre style="font-size: 12px; text-align: left; color: #000000; font-family: 'Courier New', Courier, monospace; margin: 8px;">1 0 0 0 2 0</pre>
<pre style="font-size: 12px; text-align: left; color: #000000; font-family: 'Courier New', Courier, monospace; margin: 8px;"><pre style="font-size: 12px; text-align: left; color: #000000; font-family: 'Courier New', Courier, monospace; margin: 8px;"><pre style="font-size: 10px; text-align: left; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; margin: 8px;"><strong>Explanation of the sample case: </strong>the process goes like this:&nbsp;</pre>
<pre style="font-size: 10px; text-align: left; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; margin: 8px;">(1 0 0 0 2 0) - (3 1 3 3 3 2) - (13 12 12 12 14 12)</pre>
</pre>
</pre>
</pre>
</pre>