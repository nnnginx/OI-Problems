<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;You are on vacation on a drunken island, but you couldn't resist the temptation of solving a good old problem. It all started when a group of kids played a game they call "The Falling Coconuts". In this game, a number of coconuts fall to the ground, one by one, on a single axis, at the locations given in drops. If a coconut X lands on the ground, it remains where it is. If it lands on top of another coconut Y, one of the following things happens:&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- If coconut Y is surrounded on both sides by coconuts (denoted by 'O'), coconut X remains where it is.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;X</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; OYO</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- If there is no coconut directly to the right of coconut Y, coconut X slides down to the position directly to the right of coconut Y.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;X</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; OY &nbsp; -&gt; &nbsp;OYX</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;X</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;Y &nbsp; -&gt; &nbsp; YX</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- If there is a coconut directly to the right of coconut Y, but no coconut directly to the left of coconut Y, coconut X slides down to the position directly to the left of coconut Y.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;X</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp;YO &nbsp;-&gt; &nbsp;XYO</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each time coconut X slides down to a different position, it will continue to slide (following the behavior outlined above) until it's in a place where it will not slide any further.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The task is to display the final coconut configuration.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;</div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;You are on vacation on a drunken island, but you couldn't resist the temptation of solving a good old problem. It all started when a group of kids played a game they call "The Falling Coconuts". In this game, a number of coconuts fall to the ground, one by one, on a single axis, at the locations given in drops. If a coconut X lands on the ground, it remains where it is. If it lands on top of another coconut Y, one of the following things happens:&nbsp;</p>
<p>&nbsp;</p>
<p>- If coconut Y is surrounded on both sides by coconuts (denoted by 'O'), coconut X remains where it is.</p>
<p>&nbsp; &nbsp; &nbsp;X</p>
<p>&nbsp; &nbsp; OYO</p>
<p>- If there is no coconut directly to the right of coconut Y, coconut X slides down to the position directly to the right of coconut Y.</p>
<p>&nbsp; &nbsp; &nbsp;X</p>
<p>&nbsp; &nbsp; OY &nbsp; -&gt; &nbsp;OYX</p>
<p>&nbsp; &nbsp; &nbsp;X</p>
<p>&nbsp; &nbsp; &nbsp;Y &nbsp; -&gt; &nbsp; YX</p>
<p>- If there is a coconut directly to the right of coconut Y, but no coconut directly to the left of coconut Y, coconut X slides down to the position directly to the left of coconut Y.</p>
<p>&nbsp; &nbsp; &nbsp;X</p>
<p>&nbsp; &nbsp; &nbsp;YO &nbsp;-&gt; &nbsp;XYO</p>
<p>Each time coconut X slides down to a different position, it will continue to slide (following the behavior outlined above) until it's in a place where it will not slide any further.&nbsp;</p>
<p>The task is to display the final coconut configuration.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line is t = number of test cases.</p>
<p>Each test case consists of 2 lines , first line conataining the number of coconuts and second line contains n integers denoting the position of each cocnut on the x-axis.&nbsp;</p>
<h3>Output</h3>
<p>As described in the problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>8</pre>
<pre>8 9 10 11 12 8 12 10</pre>
<pre>10</pre>
<pre>6 8 10 7 9 8 8 8 8 8
<strong>Output:</strong></pre>
<pre><strong><pre style="font-weight: normal;">---O---</pre>
<pre style="font-weight: normal;">OOOOOOO</pre>
<pre style="font-weight: normal;"><pre> --O---</pre>
</pre>
<pre style="font-weight: normal;"><pre>-OOO--</pre>
</pre>
<pre>OOOOOO</pre>
</strong></pre>
<pre><strong>Explanation of test case 1:</strong></pre>
<pre>The configuration after each fallen coconut is given below:
                                                                         <span style="white-space: pre;">				</span>  X
X  -&gt;  OX  -&gt;  OOX  -&gt;  000X  -&gt;  0000X  -&gt;  X00000  -&gt;  000000X  -&gt;  0000000
In this diagram, 'X' denotes the last fallen coconut.
</pre>