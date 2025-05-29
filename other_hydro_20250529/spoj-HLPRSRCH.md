<p>A scientist was doing a research on some kinds of bacteria. He found that the kinds, he examined, take <strong>T</strong> unit of time to grow (be <span id="result_box" lang="en"><span>mature</span></span>) enough in order to can reproduce.<br><br>Also he found that each type reproduces with a constant rate which is <strong>N</strong> new bacteria every <strong>F</strong> unit of time.</p>
<p>(where <strong>F</strong>=<strong>T</strong>)</p>
<p>&nbsp;</p>
<h3>Task</h3>
<p>write a progam that reads <strong>L</strong> (number of bacteria (at the begining of the experiment)), <strong>M</strong> (number of mature bacteria of them), <strong>T</strong> (time of each to get mature which is also the time needed for reproducing <strong>N</strong> new bacteria), <strong>N</strong> (rate of reproducing per <strong>T</strong> unit of time) and <strong>Z</strong> (period elapsed by the experiment).</p>
<p>Calculate the number of bacteria after <strong>Z</strong> unit of time.Regardless of life-span</p>
<h3>Constraints</h3>
<p>1 �� <strong>L</strong> �� 5 &nbsp; &nbsp; number of bacteria (at the begining of the experiment)</p>
<p>1 �� <strong>M</strong> �� <strong>L</strong> &nbsp;&nbsp; number of mature bacteria</p>
<p>1 �� <strong>T</strong> �� 5&nbsp;&nbsp; time of each to get mature which is also the time needed for reproducing <strong>N</strong> new bacteria</p>
<p>1 �� <strong>N</strong> �� 50 &nbsp;&nbsp; rate of reproducing per <strong>T</strong> unit of time</p>
<p>1 �� <strong>Z/T</strong> �� 4,300&nbsp;&nbsp;&nbsp; period elapsed by the experiment</p>
<h3>Note</h3>
<p><strong>Z</strong> is always divisible by <strong>T</strong>.</p>
<h3>Input</h3>
<ul>
<li><strong>L</strong> (number of bacteria (at the begining of the experiment))</li>
<li><strong>M</strong> (number of mature bacteria of them)</li>
<li><strong>T</strong> (time of each to get mature which is also the time needed for reproducing <strong>N</strong> new bacteria)</li>
<li><strong>N</strong> (rate of reproducing per <strong>T</strong> unit of time)</li>
<li><strong>Z</strong> (period elapsed by the experiment)</li>
</ul>
<h3>Output</h3>
<ul>
<li>the number of bacteria after <strong>Z</strong> unit of time.Regardless of life-span.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>2<br>3<br>1<br>3<br><br><strong>Output:</strong><br>5<br><br>The experiment begins with 2 mature bacteria and one unmature bacterium.<br>For, each of the mature bacteria reproduces after 3 units of time.<br>Then th total becomes 4 -as each one got a new one (2*2)-.<br>But, for the unmature bacterium after 3 units of time, it only become mature.<br>After all of that the experiment finishes with 5 bacteria.<br><br><br><pre><strong>Input</strong><br>2<br>0<br>1<br>1<br>100<br><br><strong>Output:</strong><br>1146295688027634168202<br><br></pre>
</pre>