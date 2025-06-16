<p>Askar is planning to steal some gold from the golden river of Slovakistan! The river forms at (0,0) and flows in the north east direction - the line <strong>y = x</strong>.</p>
<p>The river is well protected by the king's army, which is sure to give chase after him. As such, he came up with an ingenious plan - he will fly a helicopter, zig-zagging in order to shake off any pursuers. Askar will start at (0,0) and fly <strong>d<sub>x</sub> </strong>meters east, then <strong>d<sub>y </sub></strong>meters north, then <strong>d<sub>x</sub> </strong>meters east, then <strong>d<sub>y </sub></strong>meters north, ... forever.</p>
<p>Of course, he will only have a small window of opportunity to extract some gold from the river every time he crosses (or touches) it. He has yet to decide the exact values of <strong>d<sub>x</sub> </strong>and <strong>d<sub>y</sub> </strong>- some might give him better chances at a successful escape, others will allow him to grab more loot.</p>
<p>Help Askar and tell him how much he can get away with for each plan.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü T ¡Ü 1000</strong> - the number of plans.</p>
<p><strong>T</strong> lines follow, each containing two integers <strong>1&nbsp;¡Ü d<sub>x</sub></strong>,<strong> d<sub>y</sub> ¡Ü 10<sup>15</sup></strong>.</p>
<h3>Output</h3>
<p>Output a single integer - the number of times Askar would cross the golden river.</p>
<p>If Askar crosses the river an infinite number of times, output <strong>-1</strong> instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1 1<br>3 2

<strong>Output:</strong>
-1<br>1 <br><br></pre>
<p><img title="Sample depictions" src="./22670/file/aniqIGrR.png" alt="Sample depictions" width="844" height="414"></p>