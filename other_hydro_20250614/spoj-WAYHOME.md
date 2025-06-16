<p>Late in the night, a group of people are approaching&nbsp;home after an exciting adventure in the wilderness. However, as a last challenge on their long and tiresome fare, they have to cross a small bridge over a raging river.</p>
<p>The bridge is so narrow and slippery that the group decides only to let a maximum of two people walk on it at any given time. Also, the person or pair who is walking on the bridge, must carry the single light that the group possesses.</p>
<p>The group asks you to determine, given the amounts of time that each person takes to cross the bridge, the minimum total amount of time it'll take the entire group to cross. Notice that, when two people walk on the bridge at the same time, their crossing time is determined by the slower walker.</p>
<h3>Input</h3>
<p>First line: The number of testcases <strong>C</strong>.</p>
<p>Next <strong>C</strong> lines: The number of people in the group <strong>N</strong>, followed by <strong><strong>N</strong></strong> sorted integers <strong>A<sub>i</sub></strong>. <strong>A<sub>i</sub></strong> is the crossing time of the i-th person.</p>
<p>0 ¡Ü <strong>C</strong> ¡Ü 100; 1 ¡Ü <strong>N</strong> ¡Ü 1000; 0 ¡Ü <strong>A<sub>i</sub></strong> ¡Ü 1000.</p>
<h3>Output</h3>
<p>For each testcase, write the minimum total amount of time it'll take the group to pass.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
1 1
2 1 2
3 1 1 1
4 1 2 4 8
<strong>Output:</strong>
1
2
3
15
</pre>
<p>In the third test case, the people can cross the bridge in the following way:</p>
<ol>
<li>The first two people walk over the bridge, taking 1 time unit.</li>
<li>One person walks back over the bridge, with the light, taking 1 time unit.</li>
<li>The two people, now on the left, cross the bridge, taking 1 time unit.</li>
</ol>
<p>&nbsp;</p>