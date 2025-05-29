<p><span style="font-family: helvetica; font-size: 11pt;">A new government has come to power after the elections in Siruseri and has promptly announced that it is reassigning all catering contracts on its rail network.</span></p>
<div title="Page 1">
<div>
<div>
<p><span style="font-family: helvetica;"><span style="font-size: 11pt;">As is well known, the rail network of Siruseri is organized so that every station is connected to every other station by a unique path. The new scheme requires contractors to bid for a group of </span><span style="font-size: 11pt;">K </span><span style="font-size: 11pt;">stations at a time. However, the constraint is that all </span><span style="font-size: 11pt;">K </span><span style="font-size: 11pt;">stations that a contractor bids for must form a connected portion of the network. Having announced this, the government is now scratching its head to figure out how many different combinations of stations contractors can bid for. </span></span></p>
<p><span style="font-family: helvetica;"><span style="font-size: 11pt;">For example, suppose the rail network is as given below, and contractors have to bid for 3 stations at a time. Then, there are six possible combinations, namely </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">1</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">3</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">, </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">1</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">5</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">, </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">3</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">5</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">, </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">4</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">5</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">, </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">5</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">6</span></em><span style="font-size: 11pt;"><em>}</em> </span><span style="font-size: 11pt;">and </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">4</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">5</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">6</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">. A combination such as </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">1</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">4</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">, for instance, is not permitted because these three stations are not all connected to each other.&nbsp;</span></span></p>
</div>
</div>
</div>
<p><span style="white-space: pre;"><span style="white-space: pre;"> </span> </span><img style="margin-left: 275px; margin-right: 275px;" src="./21745/file/ApDveWOM.png" alt="graph" width="282" height="163"></p>
<p><span style="font-family: helvetica; font-size: 11pt;">You will be given a description of the rail network and the number of stations that a contractor has to bid for. You have to compute the number of different combinations of stations that the contractor can legally bid for, following the rule stipulated by the government.&nbsp;</span></p>
<h3><span style="font-family: helvetica;">Input</span></h3>
<div title="Page 1">
<div>
<div>
<p><span style="font-family: helvetica;"><span style="font-size: 11pt;">The first line of input consists of two integer, </span><span style="font-size: 11pt;"><em>N</em> </span><span style="font-size: 11pt;">and </span><span style="font-size: 11pt;"><em>K</em></span><span style="font-size: 11pt;">, where </span><span style="font-size: 11pt;"><em>N</em> </span><span style="font-size: 11pt;">is the number of stations in the network and </span><span style="font-size: 11pt;"><em>K</em> </span><span style="font-size: 11pt;">is the number of stations that each bid must contain. The stations are numbered </span><em><span style="font-size: 11pt;">{</span><span style="font-size: 11pt;">1</span><span style="font-size: 11pt;">,</span><span style="font-size: 11pt;">2</span><span style="font-size: 11pt;">,...,N</span><span style="font-size: 11pt;">}</span></em><span style="font-size: 11pt;">. The next </span><span style="font-size: 11pt;"><em>N</em></span><span style="font-size: 11pt;">−</span><span style="font-size: 11pt;">1 lines describe the track segments. Each of these lines contains two integers </span><span style="font-size: 11pt;"><em>i</em> </span><span style="font-size: 11pt;">and </span><span style="font-size: 11pt;"><em>j</em> </span><span style="font-size: 11pt;">describing one track segment, where </span><span style="font-size: 11pt;"><em>i</em> </span><span style="font-size: 11pt;">and </span><span style="font-size: 11pt;"><em>j</em> </span><span style="font-size: 11pt;">are the stations at either end of the segment.&nbsp;</span></span></p>
</div>
</div>
</div>
<h3><span style="font-family: helvetica;">Output</span></h3>
<div title="Page 1">
<div>
<div>
<p><span style="font-family: helvetica;"><span style="font-size: 11pt;">A single integer, denoting the number of combinations that a contractor can legally bid for. </span><span style="font-size: 11pt;">You should report your answer modulo <em>10243</em>.</span></span><span style="font-size: 11.000000pt; font-family: 'CMTI10';">&nbsp;</span></p>
<h3><span style="font-family: helvetica;">Test Data</span></h3>
<div title="Page 1">
<div>
<div>
<p><span style="font-family: helvetica;"><span style="font-size: 11pt;">In all inputs, <em>1 </em></span><em><span style="font-size: 11pt;">≤ </span><span style="font-size: 11pt;">N </span><span style="font-size: 11pt;">≤ </span></em><span style="font-size: 11pt;"><em>2500</em> and <em>1 </em></span><em><span style="font-size: 11pt;">≤ </span><span style="font-size: 11pt;">K </span><span style="font-size: 11pt;">≤ </span></em><span style="font-size: 11pt;"><em>90</em>.&nbsp;</span></span></p>
</div>
</div>
</div>
</div>
</div>
</div>
<h3><span style="font-family: helvetica;">Example</span></h3>
<p><span style="font-family: helvetica;"><strong>Input:</strong></span></p>
<pre><span style="font-size: small;">6 3
1 2
2 5
3 2
4 5
6 5</span>
</pre>
<p><span style="font-family: helvetica;"><strong>Output:</strong> </span></p>
<pre><span style="font-size: small;">6</span></pre>
<p>&nbsp;</p>